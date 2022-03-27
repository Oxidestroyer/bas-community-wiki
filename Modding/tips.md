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


<div style='position:relative; padding-bottom:calc(102.32% + 44px)'><iframe src='https://gfycat.com/ifr/SplendidPhysicalBactrian' frameborder='0' scrolling='no' width='100%' height='100%' style='position:absolute;top:0;left:0;' allowfullscreen></iframe></div>
