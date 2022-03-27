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


## How to create an audio container


<div class='gfyitem' data-controls='false' data-expand='true' data-id='#{splendidphysicalbactrian}'></div>
