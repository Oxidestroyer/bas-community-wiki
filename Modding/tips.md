# Tips


## Unsubscribe to events
Remember to unsubscribe -= to your events. Forgetting to do so can cause memory leaks 🤯 

```csharp
public class MyLevelModule : LevelModule
{
        public override IEnumerator OnLoadCoroutine() {
            EventManager.onCreatureKill += EventManager_onCreatureKill;
            EventManager.onPossess += EventManager_onPossess;
            EventManager.onUnpossess += EventManager_onUnpossess;
        }

        public override void OnUnload()
        {
            EventManager.onCreatureKill -= EventManager_onCreatureKill;
            EventManager.onPossess -= EventManager_onPossess;
            EventManager.onUnpossess -= EventManager_onUnpossess;
        }
}
```

## To get custom weapons to sit properly on a weapon rack

Create a second `HolderPoint` (Transform) like in the pictures below.
Then add an additional `HolderPoint` on the item script named **HolderRackTopAnchor** for the weapon rack and **HolderRackTopAnchorBow** for the bow rack and reference your new `HolderPoint`.

![](https://media.discordapp.net/attachments/516724791877828631/914506834344312833/sword_on_rack.jpg)
![](https://media.discordapp.net/attachments/516724791877828631/914506834570788864/bow_on_rack.jpg)
![](https://media.discordapp.net/attachments/516724791877828631/914506834763714630/sword_holderpoint_script.PNG)
![](https://media.discordapp.net/attachments/516724791877828631/914506834944098364/bow_holderpoint_script.PNG)

## How to create an audio container


<div style='position:relative; padding-bottom:calc(102.32% + 44px)'><iframe src='https://gfycat.com/ifr/SplendidPhysicalBactrian' frameborder='0' scrolling='no' width='100%' height='100%' style='position:absolute;top:0;left:0;' allowfullscreen></iframe></div>

## Use regions in C# code to collapse regions of code together

```csharp
    public class MyLevelModule : LevelModule {
        #region onLoadlogic
        public override IEnumerator OnLoadCoroutine() {
        
            return base.OnLoadCoroutine();
        }
        #endregion
    }
```
<div style='position:relative; padding-bottom:calc(102.32% + 44px)'><iframe src='https://gfycat.com/ifr/ambitiousseveralgermanpinscher' frameborder='0' scrolling='no' width='100%' height='100%' style='position:absolute;top:0;left:0;' allowfullscreen></iframe></div>

