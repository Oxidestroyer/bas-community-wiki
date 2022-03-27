# Snippets


## U10


#### Spawning a prefab asynchronously from an asset bundle


```csharp
Catalog.InstantiateAsync<GameObject>("myPrefabGameObject", myGameObject => {
  myGameObject.transform.position = whatever;
}, "SpawningMyGameObject");
```

#### Is Player holding an Item with Telekinesis
```csharp
/// <summary>
/// Returns true if the player is TK holding the item
/// </summary>
/// <param name="item"></param>
/// <returns></returns>
public static bool IsPlayerTkHolding( Item item ) {
    if ( item != null ) {
        foreach ( SpellCaster spellCaster in item.tkHandlers ) {
            if ( spellCaster.ragdollHand.creature.isPlayer ) {
                return true;
            }
        }
    }
    return false;
}
```

#### Disable culling for an Item (uses reflection)
```csharp
item.Set("cullingDetectionEnabled", false);
 
public static void Set<T>( this object source, string fieldName, T val ) {
    source.GetType()
        .GetField(fieldName, BindingFlags.NonPublic | BindingFlags.Instance)
        .SetValue(source, val);
}
```


#### Basic U10 LevelModule json
```json
{
  "$type": "ThunderRoad.LevelData, ThunderRoad",
  "id": "Master",
  "version": 3,
  "modes": [
    {
      "name": "Default",
      "modules": [
        {
          "$type": "Namespace.Classname, DLL-Name"
        }
      ]
    }
  ]
}
```

## Adding custom tips

Create a level module which on load adds your tips to the catalog at runtime.
This will add them to the base game tips without overwriting them or other modders ones.

```csharp
    public class AddLoadingScreenTips : LevelModule {
        public List<string> tips = new List<string> {
            "Tip1",
            "Tip2",
            "Tip3"
        };
        public override IEnumerator OnLoadCoroutine() {
            AddTips();
            return base.OnLoadCoroutine();
        }
        private void AddTips() {
            var textData = Catalog.GetTextData();
            if ( textData.GetGroup("Tips") != null ) {
                var tips = textData.GetGroup("Tips");
                int id = tips.texts.Count;
                foreach ( string t in this.tips ) {
                    id++;
                    var tip = new TextData.TextID {
                        id = id.ToString(),
                        text = t
                    };
                    tips.texts.Add(tip);
                }
            }
        }
    }
```

## Basic U10 LiquidData class

Allows to make scripts for potions. Reference it in a Liquid JSON. Remember it runs about every second the liquid touches a creature's head. Place your code where "//Code here" is, the rest is mostly there to make the potion blots appear.

```csharp
public override void OnLiquidReception(
      LiquidReceiver liquidReceiver,
      float dilution,
      LiquidContainer liquidContainer)
    {
      if (!liquidReceiver.collisionHandler.isRagdollPart)
        return;

      //Code here

      List<RevealMaterialController> bodyRevealRmc = new List<RevealMaterialController>();
      List<RevealMaterialController> outfitRmc = new List<RevealMaterialController>();
      foreach (Creature.RendererData renderer in liquidReceiver.collisionHandler.ragdollPart.ragdoll.creature.renderers)
      {
        if ((bool) (UnityEngine.Object) renderer.revealDecal && (bool) (UnityEngine.Object) renderer.revealDecal.revealMaterialController)
        {
          if (renderer.revealDecal.type == RevealDecal.Type.Body)
            bodyRevealRmc.Add(renderer.revealDecal.revealMaterialController);
          else if (renderer.revealDecal.type == RevealDecal.Type.Outfit)
            outfitRmc.Add(renderer.revealDecal.revealMaterialController);
        }
      }
      if (this.blitCoroutine != null)
        liquidReceiver.StopCoroutine(this.blitCoroutine);
      this.blitCoroutine = liquidReceiver.StartCoroutine(this.BlitCoroutine(bodyRevealRmc, outfitRmc, liquidReceiver.collisionHandler.ragdollPart.ragdoll.creature, dilution));
    }
```
