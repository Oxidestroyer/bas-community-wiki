# ThunderRoad

## `AndroidExporter`

```csharp
public class ThunderRoad.AndroidExporter
    : MonoBehaviour

```

## `AnimationData`

```csharp
public class ThunderRoad.AnimationData
    : CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Clip>` | animationClips |  | 
| `Boolean` | autoMinMaxRange |  | 
| `Single` | maxRange |  | 
| `Single` | minRange |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CalculateWeight() |  | 
| `void` | CalculateWeightDelta(`Single` targetDistance, `Single` movedDistance, `Single` maxdelta, `Single` animSpeedMult) |  | 
| `List<ValueDropdownItem<String>>` | GetAllAnimationDataID() |  | 
| `void` | OnCatalogRefresh() |  | 
| `Clip` | Pick(`Direction` moveDirection) |  | 
| `Clip` | Pick(`Direction` moveDirection, `Direction` aimDirection) |  | 
| `Clip` | Pick(`Step` step) |  | 
| `Clip` | PickDeltaRNG(`Single` targetDistance, `Single` movedDistance, `Single` maxdelta, `Single` animSpeedMult = 1) |  | 
| `Clip` | PickRNG() |  | 


## `AnimationTester`

```csharp
public class ThunderRoad.AnimationTester
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | timeScale |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CastLeft() |  | 
| `void` | Choke() |  | 
| `void` | Electrocute() |  | 
| `void` | StanceBow() |  | 
| `void` | StanceIdle() |  | 
| `void` | StanceOneHanded() |  | 
| `void` | StanceShield() |  | 
| `void` | StanceStaff() |  | 
| `void` | Tpose() |  | 


## `AudioContainer`

```csharp
public class ThunderRoad.AudioContainer
    : ScriptableObject

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioClip[]` | filteredSounds |  | 
| `Int32` | filteredSoundsCount |  | 
| `Boolean` | filteredSoundsInitialized |  | 
| `AudioClip` | lastPlayedClip |  | 
| `List<AudioClip>` | sounds |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | FilterClips(`List<AudioClip>` audioClips) |  | 
| `AudioClip` | GetRandomAudioClip(`List<AudioClip>` audioClips) |  | 
| `AudioClip` | PickAudioClip() |  | 
| `AudioClip` | PickAudioClip(`Int32` index) |  | 


## `AudioLoader`

```csharp
public class ThunderRoad.AudioLoader
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | audioClipAddress |  | 
| `AssetReferenceT<AudioClip>` | audioClipReference |  | 
| `AudioMixerName` | audioMixer |  | 
| `AudioSource` | audioSource |  | 
| `Boolean` | useAudioClipAddress |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | OnDisable() |  | 
| `void` | OnDungeonGenerated(`EventTime` eventTime) |  | 
| `void` | OnEnable() |  | 


## `AudioMixerLinker`

```csharp
public class ThunderRoad.AudioMixerLinker
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioMixerName` | audioMixer |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 


## `AudioMixerName`

```csharp
public enum ThunderRoad.AudioMixerName
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | Master |  | 
| `1` | Effect |  | 
| `2` | Ambient |  | 
| `3` | UI |  | 
| `4` | Voice |  | 
| `5` | Music |  | 
| `6` | SlowMotion |  | 


## `AudioThrow`

```csharp
public class ThunderRoad.AudioThrow
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioSource` | audioSource |  | 
| `Item` | item |  | 
| `Single` | maxPitch |  | 
| `Single` | maxVelocity |  | 
| `Single` | minPitch |  | 
| `Rigidbody` | rigidBody |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | OnDisable() |  | 
| `void` | OnEnable() |  | 
| `void` | OnObjectReleased(`Handle` handle, `RagdollHand` ragdollHand, `Boolean` forSnap) |  | 
| `void` | OnValidate() |  | 


## `AxisDirection`

```csharp
public enum ThunderRoad.AxisDirection
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | None |  | 
| `1` | Up |  | 
| `2` | Down |  | 
| `3` | Left |  | 
| `4` | Right |  | 


## `BipedIKCustom`

```csharp
public class ThunderRoad.BipedIKCustom
    : BipedIK

```

Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `UpdateDelegate` | OnPostUpdateEvent |  | 
| `UpdateDelegate` | OnPreUpdateEvent |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | UpdateSolver() |  | 


## `BowString`

```csharp
public class ThunderRoad.BowString
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Animation` | animation |  | 
| `Single` | animationClipLength |  | 
| `Vector3` | arrowShootDirection |  | 
| `AudioClip` | audioClipString |  | 
| `AudioContainer` | audioContainerDraw |  | 
| `AudioContainer` | audioContainerShoot |  | 
| `AudioSource` | audioSourceShoot |  | 
| `AudioSource` | audioSourceString |  | 
| `Single` | currentPull |  | 
| `Boolean` | drawAudioPlayed |  | 
| `Boolean` | isPulling |  | 
| `Item` | item |  | 
| `Single` | lastNockTime |  | 
| `Item` | lastShootedArrow |  | 
| `Single` | lastShootVelocity |  | 
| `Single` | maxDrawDistance |  | 
| `Single` | minPull |  | 
| `ItemModuleBow` | module |  | 
| `Item` | nockedArrow |  | 
| `ConfigurableJoint` | nockJoint |  | 
| `Single` | nockUnockDelay |  | 
| `Vector3` | orgBowStringPos |  | 
| `Single` | previousPull |  | 
| `Single` | pullMultiplier |  | 
| `Single` | pullOffset |  | 
| `Transform` | rest |  | 
| `Single` | restArrowLocalPosZ |  | 
| `Item` | restedArrow |  | 
| `ConfigurableJoint` | restJoint |  | 
| `Transform` | restLeft |  | 
| `Transform` | restRight |  | 
| `Boolean` | shootUnrest |  | 
| `Vector3` | startLocalPos |  | 
| `Single` | stepPull |  | 
| `Handle` | stringHandle |  | 
| `ConfigurableJoint` | stringJoint |  | 
| `Single` | ungrabExceedDistance |  | 
| `Single` | unnockOffset |  | 
| `Single` | unnockVelocity |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Rigidbody` | rb |  | 


Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `ShootDelegate` | OnShootEvent |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | NockArrow(`Handle` arrowHandle, `HandleOrientation` handleOrientation = null) |  | 
| `void` | ReleaseArrow() |  | 
| `void` | ResetStringSpring() |  | 
| `void` | SetFrame(`Single` frame) |  | 
| `void` | SetJointMotion(`ConfigurableJointMotion` configurableJointMotion) |  | 
| `void` | SetStringSpring(`Single` spring) |  | 
| `void` | Unnock() |  | 
| `void` | Unrest() |  | 


## `Brain`

```csharp
public class ThunderRoad.Brain
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | canDamage |  | 
| `Creature` | creature |  | 
| `Stagger` | currentStagger |  | 
| `Creature` | currentTarget |  | 
| `BrainData` | instance |  | 
| `Boolean` | isAttacking |  | 
| `Boolean` | isCarried |  | 
| `Boolean` | isCasting |  | 
| `Boolean` | isChoke |  | 
| `Boolean` | isDying |  | 
| `Boolean` | isElectrocuted |  | 
| `Boolean` | isParrying |  | 
| `NavMeshAgent` | navMeshAgent |  | 
| `List<Object>` | noStandupModifiers |  | 
| `List<Zone>` | slowZones |  | 
| `State` | state |  | 


Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `AttackEvent` | OnAttackEvent |  | 
| `PushEvent` | OnPushEvent |  | 
| `Action<State>` | OnStateChangeEvent |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddNoStandUpModifier(`Object` handler) |  | 
| `void` | Awake() |  | 
| `Boolean` | CanSight(`Vector3` targetPosition, `Single` sightThickness, `Single` minDistance, `Single` maxDistance, `Boolean` showDebugLines = False) |  | 
| `Boolean` | CanSight(`Creature` targetCreature, `Boolean` useDetectionMaxDistance = False, `Boolean` showDebugLines = False) |  | 
| `Boolean` | CanSight(`Creature` targetCreature, `RagdollPart&` sightedRagdollPart, `Boolean` useDetectionMaxDistance = False, `Boolean` showDebugLines = False) |  | 
| `Boolean` | CanSight(`Creature` targetCreature, `Single` sightThickness, `Single` minDistance, `Single` maxDistance, `Boolean` showDebugLines = False) |  | 
| `Boolean` | CanSight(`Creature` targetCreature, `Single` sightThickness, `Single` minDistance, `Single` maxDistance, `RagdollPart&` sightedRagdollPart, `Boolean` showDebugLines = False) |  | 
| `void` | ClearNoStandUpModifiers() |  | 
| `Single` | GetDistance(`Transform` target) |  | 
| `Single` | GetDistance(`Vector3` targetPosition) |  | 
| `Int32` | GetFreeAvoidancePriority(`Int32` avoidancePriority) |  | 
| `Single` | GetHeight(`Transform` target) |  | 
| `Single` | GetHorizontalAngle(`Transform` target) |  | 
| `Single` | GetHorizontalDistance(`Transform` target) |  | 
| `Single` | GetHorizontalDistance(`Vector3` targetPosition) |  | 
| `void` | Init(`Creature` creature) |  | 
| `void` | InvokeAttackEvent(`AttackType` attackType, `Boolean` strong, `Creature` target) |  | 
| `void` | InvokePushEvent(`PushType` type, `Stagger` stagger) |  | 
| `void` | Load(`String` brainId) |  | 
| `void` | OnCreatureDespawn(`EventTime` eventTime) |  | 
| `void` | OnCreatureDisable() |  | 
| `void` | OnCreatureEnable() |  | 
| `void` | OnDrawGizmos() |  | 
| `void` | OnDrawGizmosSelected() |  | 
| `void` | OnRagdollStateChange(`State` previousState, `State` newState, `PhysicStateChange` physicStateChange, `EventTime` eventTime) |  | 
| `void` | OnZoneEvent(`Zone` zone, `Boolean` enter) |  | 
| `void` | RemoveNoStandUpModifier(`Object` handler) |  | 
| `void` | SetState(`State` newState) |  | 
| `void` | Stop() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | hashAim |  | 
| `Int32` | hashBlock |  | 
| `Int32` | hashCarry |  | 
| `Int32` | hashCast |  | 
| `Int32` | hashCastCurve |  | 
| `Int32` | hashCastSide |  | 
| `Int32` | hashChoke |  | 
| `Int32` | hashDodge |  | 
| `Int32` | hashDodgeType |  | 
| `Int32` | hashElectrocute |  | 
| `Int32` | hashHit |  | 
| `Int32` | hashHitDirX |  | 
| `Int32` | hashHitDirY |  | 
| `Int32` | hashHitType |  | 
| `Boolean` | hashInitialized |  | 
| `Int32` | hashInjured |  | 
| `Int32` | hashIsCastingLeft |  | 
| `Int32` | hashIsCastingRight |  | 
| `Int32` | hashIsReloading |  | 
| `Int32` | hashIsShooting |  | 
| `Int32` | hashParryMagic |  | 
| `Int32` | hashReload |  | 
| `Int32` | hashShoot |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | InSightRange(`Vector3` fromPosition, `Vector3` toPosition, `Single` sightThickness, `Single` minDistance, `Single` maxDistance, `Boolean` showDebugLines = False) |  | 


## `BrainData`

```csharp
public class ThunderRoad.BrainData
    : CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Creature` | creature |  | 
| `Boolean` | cycle |  | 
| `Single` | cyclePlayerMaxDistance |  | 
| `Single` | cyclePlayerMinDistance |  | 
| `Single` | cycleSpeed |  | 
| `Int32` | difficulty |  | 
| `Boolean` | hasTree |  | 
| `Boolean` | isActive |  | 
| `Single` | lastCycleTime |  | 
| `List<Module>` | modules |  | 
| `BehaviorTreeData` | tree |  | 
| `Boolean` | treeDebugLog |  | 
| `String` | treeID |  | 
| `Boolean` | updateTree |  | 
| `List<Action>` | updateTreeNodes |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<ValueDropdownItem<String>>` | GetAllBehaviorTreeID() |  | 
| `Int32` | GetCurrentVersion() |  | 
| `T` | GetModule(`Boolean` autoAddModuleIfMissing = True) |  | 
| `Boolean` | HasModuleUsing(`Boolean` head = False, `Boolean` armLeft = False, `Boolean` armRight = False, `Boolean` torso = False, `Boolean` legs = False) |  | 
| `BrainData` | Instantiate() |  | 
| `void` | LateUpdate() |  | 
| `void` | Load(`Creature` creature) |  | 
| `void` | OnDrawGizmos() |  | 
| `void` | OnDrawGizmosSelected() |  | 
| `void` | Start() |  | 
| `void` | Stop() |  | 
| `void` | StopModuleUsing(`Boolean` head = False, `Boolean` armLeft = False, `Boolean` armRight = False, `Boolean` torso = False, `Boolean` legs = False) |  | 
| `void` | StopModuleUsingAnyBodyPart() |  | 
| `void` | Unload() |  | 
| `void` | Update(`Boolean` force = False) |  | 


## `BrainModuleBow`

```csharp
public class ThunderRoad.BrainModuleBow
    : Module

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | aimHitDropDelay |  | 
| `Vector3` | aimMovePosOffset |  | 
| `Single` | aimRotationAngle |  | 
| `Single` | aimSpeed |  | 
| `Single` | aimSpreadAngle |  | 
| `Vector3` | aimStaticPosOffset |  | 
| `Single` | arrowDrawDelay |  | 
| `Single` | arrowNockDelay |  | 
| `Vector2` | bowAimMinMaxDelay |  | 
| `Single` | bowDrawDelay |  | 
| `Single` | maxAimAngle |  | 
| `Single` | maxPullRatio |  | 
| `Single` | maxShootAngle |  | 
| `Vector2` | shootMinMaxDelay |  | 
| `Single` | shootVelocity |  | 
| `Single` | turnSpeed |  | 


## `BrainModuleCast`

```csharp
public class ThunderRoad.BrainModuleCast
    : Module

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | aimArmLenghtMultiplier |  | 
| `Vector2` | castMinMaxDelay |  | 
| `Single` | delayIk |  | 
| `Vector2` | longRangeMinMaxDist |  | 
| `Single` | maxAimAngle |  | 
| `Single` | maxFireAngle |  | 
| `Vector2` | midRangeMinMaxDist |  | 
| `Single` | minMana |  | 
| `Vector2` | shortRangeMinMaxDist |  | 
| `Vector2` | spreadCone |  | 
| `Boolean` | usePositionIK |  | 
| `Boolean` | useRotationIK |  | 


## `BrainModuleDeath`

```csharp
public class ThunderRoad.BrainModuleDeath
    : Module

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `CollisionInstance` | collisionInstance |  | 
| `Coroutine` | coroutine |  | 
| `AnimationCurve` | curve |  | 
| `AnimationData` | defaultAnimationData |  | 
| `String` | defaultAnimationId |  | 
| `Vector2` | dropObjectsDelay |  | 
| `Single` | grabThrowMinVelocity |  | 
| `Single` | maxMovingVelocity |  | 
| `Boolean` | pinPosition |  | 
| `AnimationData` | stabAnimationData |  | 
| `String` | stabAnimationId |  | 
| `Single` | unpinDistance |  | 
| `Single` | unpinMaxAngle |  | 
| `Boolean` | useDamagerDyingAnimMaxVelocity |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `IEnumerator` | DropGrabbedCoroutine(`Side` side) |  | 
| `List<ValueDropdownItem<String>>` | GetAllAnimationID() |  | 
| `void` | Load(`Creature` creature) |  | 
| `void` | OnDamage(`CollisionInstance` collisionInstance) |  | 
| `void` | OnKill(`CollisionInstance` collisionInstance, `EventTime` eventTime) |  | 
| `void` | StopDying() |  | 
| `void` | Unload() |  | 


## `BrainModuleDetection`

```csharp
public class ThunderRoad.BrainModuleDetection
    : Module

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Nullable<Single>` | alertednessLevel |  | 
| `Single` | alertednessLossPerSec |  | 
| `Int32` | allyAttackingCount |  | 
| `Boolean` | allyOnLeft |  | 
| `Boolean` | allyOnRight |  | 
| `Int32` | allyTotalCount |  | 
| `ParryInfo` | attackInfoLeft |  | 
| `ParryInfo` | attackInfoRight |  | 
| `Boolean` | canHear |  | 
| `Creature` | closestLeftAlly |  | 
| `Single` | closestLeftAllyDistance |  | 
| `Creature` | closestRightAlly |  | 
| `Single` | closestRightAllyDistance |  | 
| `CapsuleCollider` | defenseCollider |  | 
| `Single` | defenseColliderHeightMultiplier |  | 
| `Single` | defenseColliderRadius |  | 
| `Single` | detectAlertednessThreshold |  | 
| `Single` | enemyInFOVCycleValue |  | 
| `Single` | hearMaxDistance |  | 
| `Single` | hearMinNoiseRatio |  | 
| `Single` | hearRememberDuration |  | 
| `Int32` | lastCheckCloseFriendsFrame |  | 
| `Creature` | lastCheckCloseFriendsTarget |  | 
| `Int32` | lastIncomingStrikeCheckFrame |  | 
| `Boolean` | lastIncomingStrikeResult |  | 
| `Creature` | lastStrikeIncomingTarget |  | 
| `Single` | sightDetectionFov |  | 
| `Single` | sightMaxHeight |  | 
| `Single` | soundHeardScalableCycleValue |  | 
| `Boolean` | underSpellFire |  | 
| `Single` | underSpellFireMaxAngle |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | AlertednessThresholdCheck(`Single` alertednessIncrease) |  | 
| `void` | CheckAllies(`Creature` targetCreature) |  | 
| `Boolean` | CheckCreaturesBreakThreshold(`List<Creature>` enemiesSeen) |  | 
| `Boolean` | CheckIncomingStrike(`Creature` targetCreature) |  | 
| `Boolean` | CheckSoundBreaksThreshold(`Single` loudnessRatio) |  | 
| `Creature` | GetClosestTarget(`Single&` distance) |  | 
| `void` | Load(`Creature` creature) |  | 
| `void` | OnCycle() |  | 
| `void` | OnDrawGizmos() |  | 
| `void` | Update() |  | 
| `void` | UpdateUnderSpellFire(`Creature` targetCreature) |  | 


## `BrainModuleDodge`

```csharp
public class ThunderRoad.BrainModuleDodge
    : Module

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | active |  | 
| `DodgeBehaviour` | dodgeBehaviour |  | 
| `Single` | dodgeChance |  | 
| `Single` | dodgeForceDistance |  | 
| `Single` | dodgeMaxHeight |  | 
| `Boolean` | dodgeStabForce |  | 
| `Single` | dodgeStabMaxAngle |  | 
| `Single` | dodgeThreatDistance |  | 
| `Single` | dodgeThreatMinSpeed |  | 
| `Boolean` | dodgeWhenGrabbed |  | 
| `Boolean` | dodgeWhenWeaponGrabbed |  | 
| `Boolean` | enabled |  | 
| `BrainModuleDetection` | moduleDetection |  | 
| `Creature` | targetCreature |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CanMove(`Vector3` position, `Single` maxHeight) |  | 
| `void` | Load(`Creature` creature) |  | 
| `void` | StartDodge(`Creature` targetCreature, `DodgeBehaviour` dodgeBehaviour) |  | 
| `void` | StopDodge() |  | 
| `void` | TryToDodge(`ParryInfo` attackInfo, `DodgeBehaviour` dodgeBehaviour) |  | 
| `void` | TryToDodge(`Vector3` velocity, `Single` hitHeight, `Vector3` targetDir, `DodgeBehaviour` dodgeBehaviour) |  | 
| `void` | Update() |  | 


## `BrainModuleElectrocute`

```csharp
public class ThunderRoad.BrainModuleElectrocute
    : Module

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Coroutine` | aliveToDeathCoroutine |  | 
| `Int32` | boltCount |  | 
| `Int32` | boltHitCount |  | 
| `Single` | boltMinTime |  | 
| `Coroutine` | coroutine |  | 
| `Vector2Int` | deadRotationSpringRange |  | 
| `Single` | duration |  | 
| `Boolean` | dying |  | 
| `EffectData` | effectData |  | 
| `EffectInstance` | effectInstance |  | 
| `Int32` | imbueHitCount |  | 
| `Single` | imbueHitMinTime |  | 
| `Single` | lastBoltHitTime |  | 
| `Single` | lastElectrocuteTime |  | 
| `Single` | power |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Load(`Creature` creature) |  | 
| `void` | OnDamage(`CollisionInstance` collisionInstance) |  | 
| `void` | OnKill(`CollisionInstance` collisionInstance, `EventTime` eventTime) |  | 
| `void` | OnRagdollStateChange(`State` previousState, `State` newState, `PhysicStateChange` physicStateChange, `EventTime` eventTime) |  | 
| `void` | StopElectrocute() |  | 
| `void` | TryElectrocute(`Single` power, `Single` duration, `Boolean` forced, `Boolean` imbueHit, `EffectData` effectData = null) |  | 
| `void` | Unload() |  | 


## `BrainModuleEquipment`

```csharp
public class ThunderRoad.BrainModuleEquipment
    : Module

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | allowArmGrabDisarm |  | 
| `Boolean` | allowArmStabDisarm |  | 
| `Vector2` | dropObjectsDelay |  | 
| `Int32` | grabDisarmPushLevel |  | 
| `Int32` | handHitDisarmPushLevel |  | 
| `Boolean` | isDrawing |  | 
| `Boolean` | isHolstering |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `IEnumerator` | DrawWeaponCoroutine(`Item` rightHandWeapon, `Item` leftHandWeapon) |  | 
| `IEnumerator` | DropGrabbedCoroutine(`Side` side) |  | 
| `IEnumerator` | HolsterCoroutine(`Boolean` rightHand, `Boolean` leftHand) |  | 
| `void` | Load(`Creature` creature) |  | 
| `void` | OnBrainStart() |  | 
| `void` | OnBrainStop() |  | 
| `void` | OnDamage(`CollisionInstance` collisionInstance) |  | 
| `void` | ResetDrawAndHolster() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | drawDelay |  | 
| `Int32` | hashDrawLeft |  | 
| `Int32` | hashDrawRight |  | 
| `Boolean` | hashInitialized |  | 


## `BrainModuleGrabbed`

```csharp
public class ThunderRoad.BrainModuleGrabbed
    : Module

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | freeBothHand |  | 
| `Coroutine` | freeBothHandCoroutine |  | 
| `Single` | freeBothHandDelay |  | 
| `Boolean` | freeOneHand |  | 
| `Coroutine` | freeOneHandCoroutine |  | 
| `Single` | freeOneHandDelay |  | 
| `Single` | grabThrowMinVelocity |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | FreeBothHand() |  | 
| `void` | FreeOneHand() |  | 
| `Behaviour` | GetBehaviour() |  | 
| `void` | OnBrainStart() |  | 
| `void` | OnBrainStop() |  | 
| `void` | OnGrab(`RagdollHand` ragdollHand, `HandleRagdoll` handleRagdoll) |  | 
| `void` | OnKill(`CollisionInstance` collisionInstance, `EventTime` eventTime) |  | 
| `void` | OnRagdollStateChange(`State` previousState, `State` newState, `PhysicStateChange` physicStateChange, `EventTime` eventTime) |  | 
| `void` | OnTelekinesisGrab(`SpellTelekinesis` spellTelekinesis, `HandleRagdoll` handleRagdoll) |  | 
| `void` | OnTelekinesisRelease(`SpellTelekinesis` spellTelekinesis, `HandleRagdoll` handleRagdoll, `Boolean` lastHandler) |  | 
| `void` | OnUngrab(`RagdollHand` ragdollHand, `HandleRagdoll` handleRagdoll, `Boolean` lastHandler) |  | 
| `void` | Refresh() |  | 
| `void` | StopGrab() |  | 


## `BrainModuleHitReaction`

```csharp
public class ThunderRoad.BrainModuleHitReaction
    : Module

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | cancelGetUp |  | 
| `Coroutine` | coroutine |  | 
| `Single` | jumpFootHeightThreshold |  | 
| `Single` | knockoutDuration |  | 
| `Single` | knockoutTime |  | 
| `List<PushBehaviour>` | pushGrabThrowBehaviors |  | 
| `List<PushBehaviour>` | pushHitBehaviors |  | 
| `List<PushBehaviour>` | pushMagicBehaviors |  | 
| `Single` | staggerLight |  | 
| `Single` | staggerMedium |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `PushBehaviour` | GetBehaviour(`PushType` pushType, `Int32` level, `Type` bodyPart) |  | 
| `StaggerAnimation` | GetStaggerAnimation(`Type` bodyPart) |  | 
| `Single` | GetStaggerRecoil(`Effect` behaviourEffect) |  | 
| `void` | OnBrainStart() |  | 
| `void` | OnBrainStop() |  | 
| `void` | OnCycle() |  | 
| `void` | OnDamage(`CollisionInstance` collisionInstance) |  | 
| `void` | TryPush(`PushType` type, `Vector3` direction, `Int32` pushLevel, `Type` bodyPart) |  | 


## `BrainModuleLookAt`

```csharp
public class ThunderRoad.BrainModuleLookAt
    : Module

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | aboveClampHeight |  | 
| `Single` | aboveMaxHeight |  | 
| `Single` | aboveWeightChangeSpeed |  | 
| `Boolean` | adjustBodyWeight |  | 
| `Single` | bodyWeight |  | 
| `Single` | clampWeightBody |  | 
| `Single` | clampWeightEyes |  | 
| `Single` | clampWeightHead |  | 
| `Single` | currentClampWeightBody |  | 
| `Single` | eyesWeight |  | 
| `Single` | fadeSpeed |  | 
| `Single` | headWeight |  | 
| `Boolean` | isLooking |  | 
| `Transform` | lookAtTransform |  | 
| `Transform` | targetTransform |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Load(`Creature` creature) |  | 
| `void` | OnBrainStop() |  | 
| `void` | OnCycle() |  | 
| `void` | RefreshIK() |  | 
| `void` | SetLookAt(`Vector3` targetPosition) |  | 
| `void` | SetLookAt(`Transform` targetTransform) |  | 
| `void` | StopLookAt(`Boolean` instant = False) |  | 
| `void` | StopSameBodyPart() |  | 
| `void` | Update() |  | 


## `BrainModuleMelee`

```csharp
public class ThunderRoad.BrainModuleMelee
    : Module

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | animationSpeedMultiplier |  | 
| `Single` | armDamperMultiplier |  | 
| `Single` | armMaxForceMultiplier |  | 
| `Single` | armSpringMultiplier |  | 
| `Single` | attackMaxAngle |  | 
| `Single` | attackMaxDelay |  | 
| `Single` | attackMinDelay |  | 
| `Single` | attackTurnSpeedMultiplier |  | 
| `AnimationData` | defaultAnimationData |  | 
| `String` | defaultAnimationId |  | 
| `AnimationData` | dualAnimationData |  | 
| `String` | dualAnimationId |  | 
| `Single` | lastAttackTime |  | 
| `Single` | maxRangeDelta |  | 
| `Boolean` | meleeEnabled |  | 
| `Int32` | meleeMax |  | 
| `BrainModuleStance` | moduleStance |  | 
| `Single` | nextAttackDelay |  | 
| `Single` | recoilMinWeaponSpeed |  | 
| `Boolean` | recoilOnParry |  | 
| `AnimationData` | shieldAnimationData |  | 
| `String` | shieldAnimationId |  | 
| `AnimationData` | staffAnimationData |  | 
| `String` | staffAnimationId |  | 
| `AnimationData` | sword1hAnimationData |  | 
| `String` | sword1hAnimationId |  | 
| `Single` | weaponReachRatio |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<ValueDropdownItem<String>>` | GetAllAnimationID() |  | 
| `AnimationData` | GetAnimationData(`Stance` stance) |  | 
| `Single` | GetMaxMeleeRange() |  | 
| `Single` | GetMaxReach() |  | 
| `void` | GetMeleeRanges(`Single&` minRange, `Single&` maxRange) |  | 
| `Single` | GetMinMeleeRange() |  | 
| `Single` | GetWeaponReach() |  | 
| `void` | Load(`Creature` creature) |  | 
| `void` | OnDrawGizmosSelected() |  | 
| `Clip` | PickBestAttackAnimation(`Creature` target) |  | 


## `BrainModuleMove`

```csharp
public class ThunderRoad.BrainModuleMove
    : Module

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | acceleration |  | 
| `Boolean` | allowMove |  | 
| `Boolean` | isMoving |  | 
| `Single` | lastMoveTime |  | 
| `Single` | locomotionBackwardSpeedMultiplier |  | 
| `Boolean` | locomotionOverride |  | 
| `Single` | locomotionRunSpeedMultiplier |  | 
| `Single` | locomotionSpeedMultiplier |  | 
| `Single` | locomotionStrafeSpeedMultiplier |  | 
| `Single` | moveSpeedRatio |  | 
| `NavMeshAgent` | navMeshAgent |  | 
| `Vector3` | navPosition |  | 
| `Single` | navReachDistance |  | 
| `Single` | nextMoveDelay |  | 
| `Single` | runDistance |  | 
| `Single` | runSpeedRatio |  | 
| `Int32` | samplePositionCircleSteps |  | 
| `Single` | strafeDelay |  | 
| `Single` | strafeMaxDelay |  | 
| `Single` | strafeMinDelay |  | 
| `Single` | strafeTime |  | 
| `List<TurnRequest>` | turnRequests |  | 
| `Boolean` | useAcceleration |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3` | GetRandomPointAround(`Vector3` position, `Vector3` direction, `Single` angle, `Single` minRadius, `Single` maxRadius) |  | 
| `void` | Load(`Creature` creature) |  | 
| `void` | OnDrawGizmos() |  | 
| `void` | StopMove() |  | 
| `void` | StopTurn(`Object` handler) |  | 
| `Boolean` | TryGetTurnRequest(`Object` handler, `TurnRequest&` turnRequest) |  | 
| `Boolean` | TrySampleCirclePosition(`Vector3` position, `Single` circleMinRadius, `Single` circleMaxRadius, `Single` circleAngle, `Boolean` unobstructedPathFirst, `Vector3&` navPosition) |  | 
| `void` | TurnTo(`Vector3` direction, `Object` handler, `Single` turnSpeedRatio = 1) |  | 
| `void` | TurnTo(`Transform` transform, `Object` handler, `Single` turnSpeedRatio = 1) |  | 
| `void` | TurnToNavDirection(`Object` handler, `Single` turnSpeedRatio = 1) |  | 
| `void` | Update() |  | 
| `State` | UpdateMoveCycle(`Vector3` targetPosition, `Single` targetMinRadius, `Single` targetMaxRadius, `Single` moveSpeedRatio = 1, `Single` runSpeedRatio = 1, `Single` targetRadiusAngle = 0, `Boolean` unobstructedPathFirst = False, `Single` repathMinDelay = 0, `Single` repathMaxDelay = 0) |  | 
| `void` | UpdateTurn(`Transform` turnTarget, `Single` turnSpeedRatio) |  | 
| `void` | UpdateTurn(`Vector3` targetDirection, `Single` turnSpeedRatio) |  | 
| `void` | UpdateTurnNavDirection(`Single` turnSpeedRatio) |  | 


## `BrainModuleParry`

```csharp
public class ThunderRoad.BrainModuleParry
    : Module

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | armMaxForceMultiplier |  | 
| `Single` | armSpringMultiplier |  | 
| `Single` | defenseMinIkWeight |  | 
| `Single` | dynamicHeightOffset |  | 
| `Boolean` | enabled |  | 
| `Single` | heldDefenseMaxRadius |  | 
| `Single` | heldDefenseMinRadius |  | 
| `SideInfo` | left |  | 
| `Single` | longDefenseMaxRadius |  | 
| `Single` | longDefenseMinRadius |  | 
| `Transform` | lookAt |  | 
| `BrainModuleDetection` | moduleDetection |  | 
| `BrainModuleMelee` | moduleMelee |  | 
| `BrainModuleMove` | moduleMove |  | 
| `Single` | parryDetectionRadius |  | 
| `Single` | parryHorizontalMaxAngle |  | 
| `Single` | parryMaxDistance |  | 
| `Boolean` | parryOnSpell |  | 
| `Boolean` | parryOnThreat |  | 
| `Single` | positionSpeed |  | 
| `Single` | revertHeightRatio |  | 
| `SideInfo` | right |  | 
| `Single` | rotationSpeed |  | 
| `Creature` | targetCreature |  | 
| `Single` | turnSpeedRatio |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3` | ClosestPointOnLine(`Vector3` lineStart, `Vector3` lineEnd, `Vector3` point) |  | 
| `void` | GetClosestPoints(`Collider` collider1, `Collider` collider2, `Int32` iteration, `Vector3&` pos1, `Vector3&` pos2) |  | 
| `Transform` | GetLookAt() |  | 
| `SideInfo` | GetSideInfo(`Side` side) |  | 
| `void` | Load(`Creature` creature) |  | 
| `void` | OnBrainStop() |  | 
| `void` | OnDrawGizmos() |  | 
| `void` | OnGrab(`Side` side, `Handle` handle, `Single` axisPosition, `HandleOrientation` orientation, `EventTime` eventTime) |  | 
| `void` | OnUnGrab(`Side` side, `Handle` handle, `Boolean` throwing, `EventTime` eventTime) |  | 
| `void` | SetDefensePosition(`Side` side) |  | 
| `Boolean` | StartParry(`Creature` targetCreature) |  | 
| `void` | StopParry() |  | 
| `void` | StopSameBodyPart() |  | 
| `void` | Unload() |  | 
| `void` | Update() |  | 
| `void` | UpdateDefaultProtect(`Side` side) |  | 
| `void` | UpdateMeleeProtect(`ParryInfo` attackInfo, `Side` side, `Boolean` dual = False) |  | 


## `BrainModulePatrol`

```csharp
public class ThunderRoad.BrainModulePatrol
    : Module

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | distanceChangePoint |  | 
| `LayerMask` | obstacleMask |  | 
| `Single` | runSpeedRatio |  | 
| `LayerMask` | targetMask |  | 
| `Int32` | targetWaypointIndex |  | 
| `Single` | viewAngle |  | 
| `Single` | viewRadius |  | 
| `WayPoint[]` | waypoints |  | 


## `BrainModulePlayer`

```csharp
public class ThunderRoad.BrainModulePlayer
    : Module

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | closeCombatDistance |  | 
| `Single` | dangerDistance |  | 
| `Exposure` | exposure |  | 
| `Single` | focusGainOnDeflect |  | 
| `Single` | focusGainOnKill |  | 
| `Single` | focusGainOnParry |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnBrainStart() |  | 
| `void` | OnBrainStop() |  | 
| `void` | OnCreatureDespawn(`EventTime` eventTime) |  | 
| `void` | OnCreatureKill(`Creature` creatureKilled, `Player` player, `CollisionInstance` collisionInstance, `EventTime` eventTime) |  | 
| `void` | OnCreatureKill(`CollisionInstance` collisionInstance, `EventTime` eventTime) |  | 
| `void` | OnCreatureParry(`Creature` creatureParry, `CollisionInstance` collisionInstance) |  | 
| `void` | OnCycle() |  | 
| `void` | OnDeflect(`Creature` source, `Item` item, `Creature` target) |  | 
| `void` | SetExposure(`Exposure` newExposure) |  | 


## `BrainModuleSightable`

```csharp
public class ThunderRoad.BrainModuleSightable
    : Module

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | debug |  | 
| `Single` | lastShootUpdateDelay |  | 
| `Single` | lastShootUpdatePositionMaxDistance |  | 
| `Vector3` | lastUpdateShootPointsLocation |  | 
| `Single` | lastUpdateShootPointsTime |  | 
| `Vector3` | lastUpdateShootPositionsLocation |  | 
| `Single` | lastUpdateShootPositionsTime |  | 
| `Single` | navSamplePositionMaxDistance |  | 
| `Int32` | shootpointCount |  | 
| `ShootPoint[]` | shootpoints |  | 
| `Single` | shootPointSightThickness |  | 
| `Int32` | shootPositionCircleSteps |  | 
| `Int32` | shootPositionDepthSteps |  | 
| `Int32` | shootPositionMinRadius |  | 
| `ShootPosition[]` | shootPositions |  | 
| `List<SightableRagdollPart>` | sightableRagdollParts |  | 
| `Single` | sightDetectionMaxDistance |  | 
| `Single` | sightMaxDistance |  | 
| `Single` | sightThickness |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CheckShootPoint(`ShootPoint` shootPoint, `Single` eyeHeight) |  | 
| `Vector3` | GetPointAround(`Vector3` position, `Single` angle, `Single` radius) |  | 
| `RagdollPart` | GetSightablePart(`Vector3` fromPosition, `Single` sightThickness, `Single` minDistance, `Single` maxDistance, `Boolean` showDebugLines = False) |  | 
| `Boolean` | IsSightable(`Vector3` fromPosition, `Single` sightThickness, `Single` minDistance, `Single` maxDistance, `RagdollPart&` ragdollPart, `Boolean` showDebugLines = False) |  | 
| `Boolean` | IsSightable(`Vector3` fromPosition, `Single` sightThickness, `Single` minDistance, `Single` maxDistance, `Boolean` showDebugLines = False) |  | 
| `Boolean` | IsSightableForShoot(`Vector3` fromPosition, `Boolean` showDebugLines = False) |  | 
| `void` | Load(`Creature` creature) |  | 
| `void` | OnCycle() |  | 
| `void` | OnDrawGizmosSelected() |  | 
| `void` | Update() |  | 
| `void` | UpdateShootPoints(`Single` eyeHeight) |  | 
| `void` | UpdateShootPositions(`Single` eyeHeight) |  | 


## `BrainModuleSpeak`

```csharp
public class ThunderRoad.BrainModuleSpeak
    : Module

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | audioAttackChance |  | 
| `Single` | audioDeathChance |  | 
| `Boolean` | audioEnabled |  | 
| `Single` | audioFallVelocityThreshold |  | 
| `Single` | audioHitChance |  | 
| `Int32` | audioLipSampleDataLength |  | 
| `Single` | audioLipSyncMaxValue |  | 
| `Single` | audioLipSyncUpdateRate |  | 
| `Vector2` | audioPitchRange |  | 
| `AudioSource` | audioSource |  | 
| `Single` | audioVolume |  | 
| `Coroutine` | coroutine |  | 
| `Boolean` | fallScream |  | 
| `Boolean` | isMuffled |  | 
| `Boolean` | isSpeaking |  | 
| `Transform` | jawAnimBone |  | 
| `Single` | jawCurrentWeight |  | 
| `Quaternion` | jawOrgLocalRotation |  | 
| `Single` | jawTargetWeight |  | 
| `Single` | lastSpeakTime |  | 
| `Single` | lipSyncSpeed |  | 
| `Boolean` | loaded |  | 
| `Single` | randomSpeakAlertChance |  | 
| `Single` | randomSpeakCombatChance |  | 
| `Single` | randomSpeakDelay |  | 
| `Single` | randomSpeakIdleChance |  | 
| `Single` | randomSpeakInvestigateChance |  | 
| `Single` | speakLoudness |  | 
| `Boolean` | speakOnAttackBow |  | 
| `Boolean` | speakOnAttackCast |  | 
| `Boolean` | speakOnAttackMelee |  | 
| `Boolean` | speakOnChoke |  | 
| `VoiceData` | voiceData |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | InitAnimatorHashs() |  | 
| `void` | LateUpdate() |  | 
| `void` | Load(`Creature` creature) |  | 
| `void` | OnCycle() |  | 
| `void` | Play(`String` dialogId, `Boolean` abnormalNoise) |  | 
| `void` | Play(`Int32` dialogHashId, `Boolean` abnormalNoise, `Boolean` checkMuffled = True) |  | 
| `void` | Test(`String` dialogID, `Boolean` abnormalNoise) |  | 
| `void` | Unload() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | hashAlert |  | 
| `Int32` | hashAttackBow |  | 
| `Int32` | hashAttackCast |  | 
| `Int32` | hashAttackMelee |  | 
| `Int32` | hashChoke |  | 
| `Int32` | hashCombat |  | 
| `Int32` | hashDeath |  | 
| `Int32` | hashDeathLong |  | 
| `Int32` | hashFalling |  | 
| `Int32` | hashHit |  | 
| `Int32` | hashIdle |  | 
| `Boolean` | hashInitialized |  | 
| `Int32` | hashInvestigate |  | 
| `Int32` | hashMuffled |  | 
| `Int32` | hashMuffledDeath |  | 


## `BrainModuleStance`

```csharp
public class ThunderRoad.BrainModuleStance
    : Module

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Stance` | stance |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Load(`Creature` creature) |  | 
| `void` | OnBrainStart() |  | 
| `void` | OnBrainStop() |  | 
| `void` | OnGrab(`Side` side, `Handle` handle, `Single` axisPosition, `HandleOrientation` orientation, `EventTime` eventTime) |  | 
| `void` | OnUnGrab(`Side` side, `Handle` handle, `Boolean` throwing, `EventTime` eventTime) |  | 
| `void` | SetStance(`Stance` stance) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | hashStance |  | 


## `CameraEffects`

```csharp
public class ThunderRoad.CameraEffects
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | audioMaxPitch |  | 
| `Single` | audioMinPitch |  | 
| `AudioSource` | audioSource |  | 
| `AnimationCurve` | comfortVignetteCurve |  | 
| `Color` | damageColor |  | 
| `AnimationCurve` | flashCurve |  | 
| `Single` | flashMaxTime |  | 
| `Single` | flashMinTime |  | 
| `Color` | healColor |  | 
| `Single` | healthCurveValue |  | 
| `AnimationCurve` | heartbeatCurve |  | 
| `String` | heartBeatLoopAddress |  | 
| `AnimationCurve` | lowHealthCurve |  | 
| `Volume` | postProcessVolume |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnCreatureHeal(`Creature` creature, `Single` heal, `Creature` healer) |  | 
| `void` | OnCreatureHit(`Creature` creature, `CollisionInstance` collisionInstance) |  | 
| `void` | OnGameLoadedEvent() |  | 
| `void` | OnPossessionEvent(`Creature` creature, `EventTime` eventTime) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `ColorAdjustments` | colorAdjustments |  | 
| `Boolean` | comfortVignette |  | 
| `Boolean` | healthVignette |  | 
| `CameraEffects` | local |  | 
| `Boolean` | motionBlurActive |  | 
| `Boolean` | postProcess |  | 
| `Coroutine` | timedEffectCoroutine |  | 
| `Vignette` | vignette |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DoTimedEffect(`Color` color, `TimedEffect` timedEffect, `Single` time) |  | 
| `void` | RefreshHealth() |  | 
| `void` | RefreshPostProcess() |  | 
| `void` | RefreshPostProcess(`Boolean` activated) |  | 
| `void` | SetMotionBlur(`Boolean` active) |  | 
| `void` | SetSepia(`Single` value) |  | 
| `IEnumerator` | TimedEffectCoroutine(`Color` color, `TimedEffect` timedEffect, `Single` time) |  | 


## `CanvasFollowPlayerForward`

```csharp
public class ThunderRoad.CanvasFollowPlayerForward
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Transform` | transformToRotate |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | SetTextSpeed(`Single` aSpeed) |  | 


## `CanvasHelper`

```csharp
public class ThunderRoad.CanvasHelper
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Canvas` | canvas |  | 
| `Boolean` | canvasActive |  | 
| `Boolean` | checkVisibilityAndDistance |  | 
| `Single` | maxVisibility |  | 
| `MeshRenderer` | mesh |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CheckCamera() |  | 


## `Cardinal`

```csharp
public enum ThunderRoad.Cardinal
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | XYZ |  | 
| `1` | XZ |  | 
| `2` | X |  | 
| `3` | Z |  | 


## `Catalog`

```csharp
public static class ThunderRoad.Catalog

```

Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Advanced` | advanced |  | 
| `Boolean` | checkFileVersion |  | 
| `List`1[]` | data |  | 
| `GameData` | gameData |  | 
| `JsonSerializerSettings` | jsonSerializerSettings |  | 
| `List<String>` | loadDefaultFolders |  | 
| `List<String>` | loadModFolders |  | 
| `Boolean` | loadMods |  | 
| `Boolean` | overrideDefaultData |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `T` | EditorLoad(`String` address) |  | 
| `void` | GetAddressAndSubAddress(`String` address, `String&` addressOnly, `String&` subAddress) |  | 
| `String` | GetAddressFromPrefab(`Object` target) |  | 
| `List<String>` | GetAllID(`Category` category) |  | 
| `List<String>` | GetAllID() |  | 
| `Category` | GetCategory(`Type` type) |  | 
| `Single` | GetCollisionStayRatio(`Single` velocityMagnitude) |  | 
| `T` | GetData(`String` id, `Boolean` logError = True) |  | 
| `CatalogData` | GetData(`Category` category, `String` id, `Boolean` logError = True) |  | 
| `List<CatalogData>` | GetDataList(`Category` category) |  | 
| `List<ValueDropdownItem<String>>` | GetDropdownAllID(`Category` category, `String` noneText = None) |  | 
| `List<ValueDropdownItem<String>>` | GetDropdownAllID() |  | 
| `List<ValueDropdownItem<String>>` | GetDropdownAllTexts(`String` group, `String` noneText = None) |  | 
| `List<ValueDropdownItem<String>>` | GetDropdownHolderSlots(`String` noneText = None) |  | 
| `JsonSerializerSettings` | GetJsonNetSerializerSettings() |  | 
| `String` | GetString(`String` stringId) |  | 
| `TextData` | GetTextData() |  | 
| `Item` | GetTextItem(`String` id) |  | 
| `Page` | GetTextPage(`String` group, `Int32` id) |  | 
| `void` | InstantiateAsync(`String` address, `Action<T>` callback, `String` handlerName) |  | 
| `void` | InstantiateAsync(`IResourceLocation` location, `Action<T>` callback, `String` handlerName) |  | 
| `IEnumerator` | InstantiateCoroutine(`String` address, `Action<T>` result, `String` handlerName) |  | 
| `IEnumerator` | InstantiateCoroutine(`IResourceLocation` location, `Action<T>` result, `String` handlerName) |  | 
| `Boolean` | IsJsonLoaded() |  | 
| `Boolean` | IsSameOrSubclass(`Type` baseClass, `Type` subClass) |  | 
| `IEnumerator` | LoadAddressableAssetsCoroutine() |  | 
| `void` | LoadAllJson() |  | 
| `void` | LoadAssetAsync(`String` address, `Action<T>` callback, `String` handlerName) |  | 
| `void` | LoadAssetAsync(`IResourceLocation` location, `Action<T>` callback, `String` handlerName) |  | 
| `AsyncOperationHandle<T>` | LoadAssetAsync(`IResourceLocation` location) |  | 
| `IEnumerator` | LoadAssetCoroutine(`String` address, `Action<T>` result, `String` handlerName) |  | 
| `IEnumerator` | LoadAssetCoroutine(`IResourceLocation` location, `Action<T>` result, `String` handlerName) |  | 
| `Boolean` | LoadJson(`String` jsonText, `String` jsonPath, `String` folder) |  | 
| `void` | LoadLocationAsync(`String` address, `Action<IResourceLocation>` callback, `String` handlerName) |  | 
| `IEnumerator` | LoadLocationCoroutine(`String` address, `Action<IResourceLocation>` result, `String` handlerName) |  | 
| `void` | Refresh() |  | 
| `IEnumerator` | RefreshCoroutine() |  | 
| `void` | ReleaseAddressableAssets() |  | 
| `void` | ReleaseAsset(`AsyncOperationHandle<TObject>` handle) |  | 
| `void` | ReleaseAsset(`TObject` obj) |  | 
| `void` | ReleaseAsset(`AsyncOperationHandle` handle) |  | 
| `void` | SaveAllJson() |  | 
| `void` | SaveGameData() |  | 
| `void` | SaveToJson(`CatalogData` catalogData) |  | 


## `CatalogData`

```csharp
public class ThunderRoad.CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | filePath |  | 
| `Int32` | hashId |  | 
| `String` | id |  | 
| `String` | saveFolder |  | 
| `Int32` | version |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `CatalogData` | Clone() |  | 
| `Int32` | GetCurrentVersion() |  | 
| `List<ValueDropdownItem<String>>` | GetJsonFolders() |  | 
| `void` | Init() |  | 
| `IEnumerator` | LoadAddressableAssetsCoroutine() |  | 
| `void` | OnCatalogRefresh() |  | 
| `IEnumerator` | OnCatalogRefreshCoroutine() |  | 
| `void` | ReleaseAddressableAssets() |  | 


## `CharacterSelection`

```csharp
public class ThunderRoad.CharacterSelection
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | boolMessagePage |  | 
| `Button` | calibrateTrackerStartButton |  | 
| `GameObject` | calibrationPage |  | 
| `String` | cancelSound |  | 
| `GameObject` | canvas |  | 
| `List<PlayerCharacterData>` | characterDataList |  | 
| `AnimationClip` | characterFemalePose |  | 
| `AnimationClip` | characterMalePose |  | 
| `GameObject` | characterSelectionPage |  | 
| `Button` | characterSelectionStartButton |  | 
| `CharacterSlot` | characterSlot |  | 
| `Single` | currentFeet |  | 
| `Text[]` | currentGameModeText |  | 
| `Single` | currentInch |  | 
| `Text[]` | currentPlayerIndexText |  | 
| `Single` | currentSize |  | 
| `GameObject` | customisationPage |  | 
| `Button` | customizeButton |  | 
| `GameObject` | customizer |  | 
| `GameObject` | customizerGender |  | 
| `Button` | deleteButton |  | 
| `UISelectionListButtonsGameMode` | gameModeSelectionButton |  | 
| `GameObject` | gameModeSelectionPage |  | 
| `Boolean` | initialized |  | 
| `Transform` | leftFootBone |  | 
| `Transform` | leftFootGrip |  | 
| `UISelectionListButtonsMapSelection` | mapSelectionButton |  | 
| `UIMapLevelMode` | mapSelectionLevelMode |  | 
| `GameObject` | mapSelectionPage |  | 
| `GameObject` | messagePage |  | 
| `Vector3` | orgWaistMarkerLocalPosition |  | 
| `Quaternion` | orgWaistMarkerLocalRotation |  | 
| `Button` | playButton |  | 
| `Transform` | rightFootBone |  | 
| `Transform` | rightFootGrip |  | 
| `Transform` | rootMarker |  | 
| `List<Creature>` | spawnedPlayers |  | 
| `UISelectionListButtonsSwitchMeterImperial` | switchMeterImperial |  | 
| `String` | switchSound |  | 
| `GameObject` | tutorialMessagePage |  | 
| `String` | validationSound |  | 
| `Transform` | waistMarker |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CalibrateCharacter() |  | 
| `void` | CalibrateCharacterManually(`Boolean` useImperial = False) |  | 
| `void` | CalibrateTrackerStart() |  | 
| `void` | CalibrateTrackerValidation() |  | 
| `void` | CancelDeleteCharacter() |  | 
| `void` | CancelMapSelection() |  | 
| `void` | CancelModeSelection() |  | 
| `Boolean` | CharacterExist() |  | 
| `void` | ClearCharacter() |  | 
| `void` | ConfirmGameMode() |  | 
| `void` | ConvertImperialToMeter() |  | 
| `void` | ConvertMeterToImperial() |  | 
| `void` | CustomizeCharacter() |  | 
| `void` | CustomizerAccept() |  | 
| `void` | CustomizerCancel() |  | 
| `void` | CustomizerChangeGender(`Boolean` toMale) |  | 
| `void` | DeleteCharacter() |  | 
| `void` | DisableAllPages() |  | 
| `void` | EnablePage(`GameObject` page) |  | 
| `Creature` | GetCharacterCreature() |  | 
| `PlayerCharacterData` | GetCharacterData() |  | 
| `Int32` | GetCharacterIndex() |  | 
| `String` | GetGameMode() |  | 
| `void` | HideCharacter(`Boolean` hide) |  | 
| `IEnumerator` | InitCoroutine() |  | 
| `void` | NewCharacter() |  | 
| `void` | NextSlot() |  | 
| `void` | OnCreatureFemaleChanged() |  | 
| `void` | OnCreatureMaleChanged() |  | 
| `void` | OnDestroy() |  | 
| `void` | Play() |  | 
| `void` | PlayCancelSound() |  | 
| `void` | PlaySwitchSound() |  | 
| `void` | PlayValidationSound() |  | 
| `void` | PreviousSlot() |  | 
| `void` | RefreshCharacterHeightText() |  | 
| `void` | RefreshGameModeTexts(`GameMode` choosenGameMode) |  | 
| `void` | RefreshGender() |  | 
| `void` | RefreshSaveNumber() |  | 
| `void` | RefreshSlot() |  | 
| `void` | SelectCharacter() |  | 
| `void` | SelectSlot(`Int32` slotIndex) |  | 
| `void` | ShowDeleteCharacter() |  | 
| `void` | ShowEditPage() |  | 
| `void` | Start() |  | 
| `void` | UseTutorial(`Boolean` tutorial) |  | 
| `void` | ValidateCalibration() |  | 
| `void` | ValidateMapSelection() |  | 


## `ColliderGroup`

```csharp
public class ThunderRoad.ColliderGroup
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Collider>` | colliders |  | 
| `CollisionHandler` | collisionHandler |  | 
| `ColliderGroupData` | data |  | 
| `Imbue` | imbue |  | 
| `FxController` | imbueCustomFxController |  | 
| `String` | imbueCustomSpellID |  | 
| `Renderer` | imbueEffectRenderer |  | 
| `Renderer` | imbueEmissionRenderer |  | 
| `Transform` | imbueShoot |  | 
| `Modifier` | modifier |  | 
| `Transform` | whooshPoint |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | GenerateImbueMesh() |  | 
| `void` | Load(`ColliderGroupData` colliderGroupData) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Mesh` | GenerateIcoSphereMesh(`Int32` n, `Single` radius) |  | 


## `ColliderGroupData`

```csharp
public class ThunderRoad.ColliderGroupData
    : CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | allowPenetration |  | 
| `CollisionHandling` | collisionHandling |  | 
| `List<Modifier>` | modifiers |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Modifier` | GetModifier(`ColliderGroup` colliderGroup) |  | 
| `void` | OnCatalogRefresh() |  | 


## `CollisionHandler`

```csharp
public class ThunderRoad.CollisionHandler
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | active |  | 
| `Boolean` | checkMinVelocity |  | 
| `CollisionInstance[]` | collisions |  | 
| `Single` | customGravity |  | 
| `Boolean` | customInertiaTensor |  | 
| `CapsuleCollider` | customInertiaTensorCollider |  | 
| `Vector3` | customInertiaTensorPos |  | 
| `Quaternion` | customInertiaTensorRot |  | 
| `List<Damager>` | damagers |  | 
| `Boolean` | enterOnly |  | 
| `List<Holder>` | holders |  | 
| `Boolean` | isActive |  | 
| `Boolean` | isColliding |  | 
| `Boolean` | isItem |  | 
| `Boolean` | isRagdollPart |  | 
| `Item` | item |  | 
| `Vector3` | lastAngularVelocity |  | 
| `Vector3` | lastLinearVelocity |  | 
| `Single` | orgAngularDrag |  | 
| `Single` | orgDrag |  | 
| `Single` | orgMass |  | 
| `Single` | orgSleepThreshold |  | 
| `List<CollisionHandler>` | penetratedObjects |  | 
| `List<PhysicModifier>` | physicModifiers |  | 
| `RagdollPart` | ragdollPart |  | 
| `Rigidbody` | rb |  | 
| `Boolean` | wasColliding |  | 


Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `CollidingEvent` | OnCollidingEvent |  | 
| `CollisionEvent` | OnCollisionStartEvent |  | 
| `CollisionEvent` | OnCollisionStopEvent |  | 
| `TriggerEvent` | OnTriggerEnterEvent |  | 
| `TriggerEvent` | OnTriggerExitEvent |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | CalculateCustomInertiaTensor() |  | 
| `Vector3` | CalculateImpulseVelocity(`Collision` collision) |  | 
| `Vector3` | CalculateLastPointVelocity(`Vector3` hitPoint) |  | 
| `void` | ClearPhysicModifiers() |  | 
| `Int32` | GetFreeCollisionIndex() |  | 
| `void` | MeshRaycast(`ColliderGroup` targetColliderGroup, `Vector3` contactPoint, `Vector3` contactNormal, `Vector3` impactVelocity, `Int32&` targetPhysicMaterialHash) |  | 
| `void` | OnCollisionEnter(`Collision` collision) |  | 
| `void` | OnCollisionStay(`Collision` collision) |  | 
| `void` | OnDisable() |  | 
| `void` | RefreshPhysicModifiers() |  | 
| `void` | RemovePhysicModifier(`Object` handler) |  | 
| `void` | SetMaxCollision(`Int32` value) |  | 
| `void` | SetPhysicModifier(`Object` handler, `Int32` priority, `Single` gravityRatio = 1, `Single` massRatio = 1, `Single` drag = -1, `Single` angularDrag = -1, `Single` sleepThreshold = -1, `EffectData` effectData = null) |  | 
| `void` | SetRigidbody(`Single` mass, `Single` drag, `Single` angularDrag) |  | 
| `void` | SortDamagers() |  | 
| `void` | StopCollision(`CollisionInstance` collisionInstance) |  | 
| `void` | StopCollisions() |  | 
| `void` | Update() |  | 


## `CollisionInstance`

```csharp
public class ThunderRoad.CollisionInstance

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | active |  | 
| `SpellCaster` | casterHand |  | 
| `Vector3` | contactNormal |  | 
| `Vector3` | contactPoint |  | 
| `DamageStruct` | damageStruct |  | 
| `EffectInstance` | effectInstance |  | 
| `Boolean` | hasEffect |  | 
| `Boolean` | ignoreDamage |  | 
| `Vector3` | impactVelocity |  | 
| `Single` | intensity |  | 
| `Int32` | lastCheckFrame |  | 
| `Int32` | lastCheckFrameCount |  | 
| `Vector3` | lastRumbleSourcePoint |  | 
| `Vector3` | lastRumbleTargetPoint |  | 
| `Int32` | lastStayFrame |  | 
| `Vector3` | pressureForce |  | 
| `Vector3` | pressureRelativeVelocity |  | 
| `Collider` | sourceCollider |  | 
| `ColliderGroup` | sourceColliderGroup |  | 
| `MaterialData` | sourceMaterial |  | 
| `Collider` | targetCollider |  | 
| `ColliderGroup` | targetColliderGroup |  | 
| `MaterialData` | targetMaterial |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | IsDoneByPlayer() |  | 
| `Boolean` | IsSameSourceColliderGroup(`Collider` collider) |  | 
| `Boolean` | IsSameSourceColliderGroup(`Collider` collider, `ColliderGroup` colliderGroup) |  | 
| `Boolean` | IsSameTargetColliderGroup(`Collider` collider) |  | 
| `Boolean` | IsSameTargetColliderGroup(`Collider` collider, `ColliderGroup` colliderGroup) |  | 
| `void` | NewHit(`Collider` sourceCollider, `Collider` targetCollider, `ColliderGroup` sourceColliderGroup, `ColliderGroup` targetColliderGroup, `Vector3` impactVelocity, `Vector3` contactPoint, `Vector3` contactNormal, `Single` intensity, `MaterialData` sourceMaterial, `MaterialData` targetMaterial = null) |  | 
| `void` | ShowDebug() |  | 
| `Boolean` | SpawnEffect(`MaterialData` sourceMaterial, `MaterialData` targetMaterial, `Boolean` isOther, `EffectInstance&` effectInstanceToSpawn) |  | 
| `void` | Stay(`Collision` collision) |  | 


## `Common`

```csharp
public static class ThunderRoad.Common

```

Static Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | lightProbeVolumeLayer |  | 
| `Int32` | zoneLayer |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | ActiveInPrefabHierarchy(this `GameObject` gameObject) |  | 
| `Component` | CloneComponent(`Component` source, `GameObject` destination, `Boolean` copyProperties = False) |  | 
| `Boolean` | Contains(this `LayerMask` mask, `Int32` layer) |  | 
| `void` | DrawGizmoArrow(`Vector3` pos, `Vector3` direction, `Color` color, `Single` arrowHeadLength = 0.25, `Single` arrowHeadAngle = 20, `Boolean` dim3 = False) |  | 
| `void` | DrawGizmoCapsule(`Vector3` pos, `Vector3` direction, `Color` color, `Single` capsuleLength, `Single` capsuleRadius) |  | 
| `void` | DrawText(`GUISkin` guiSkin, `String` text, `Vector3` position, `Nullable<Color>` color = null, `Int32` fontSize = 0, `Single` yOffset = 0) |  | 
| `T` | GetClosest(`List<T>` behaviours, `Vector3` position, `Boolean` prioritizeShortestPath) |  | 
| `Transform` | GetClosest(`List<Transform>` transforms, `Vector3` position, `Boolean` prioritizeShortestPath) |  | 
| `Int32` | GetIndexByName(this `Dropdown` dropDown, `String` name) |  | 
| `Int32` | GetMaskAddLayer(`Int32` mask, `Int32` layer) |  | 
| `Int32` | GetMaskRemoveLayer(`Int32` mask, `Int32` layer) |  | 
| `String` | GetPathFromRoot(this `GameObject` obj) |  | 
| `Single` | GetPathLength(`NavMeshPath` path) |  | 
| `Platform` | GetPlatform() |  | 
| `Int32` | GetRandomWeightedIndex(`Single[]` weights) |  | 
| `Vector3` | GetRowPosition(`Transform` transform, `Int32` index, `Single` rowCount, `Single` rowSpace) |  | 
| `String` | GetStringBetween(this `String` text, `String` start, `String` end) |  | 
| `Color32` | HueColourValue(`HueColorName` color) |  | 
| `Quaternion` | InverseTransformRotation(this `Transform` transform, `Quaternion` rotation) |  | 
| `void` | MirrorChilds(this `Transform` transform, `Vector3` mirrorAxis) |  | 
| `void` | MirrorRelativeToParent(this `Transform` transform, `Vector3` mirrorAxis) |  | 
| `void` | MoveAlign(this `Transform` transform, `Transform` child, `Transform` target, `Transform` parent = null) |  | 
| `void` | MoveAlign(this `Transform` transform, `Transform` child, `Vector3` targetPosition, `Quaternion` targetRotation, `Transform` parent = null) |  | 
| `void` | SetLayerRecursively(this `GameObject` obj, `Int32` layer) |  | 
| `void` | SetParentOrigin(this `Transform` transform, `Transform` parent) |  | 
| `void` | SetParentOrigin(this `Transform` transform, `Transform` parent, `Nullable<Vector3>` localPosition = null, `Nullable<Quaternion>` localRotation = null, `Nullable<Vector3>` localScale = null) |  | 
| `Quaternion` | TransformRotation(this `Transform` transform, `Quaternion` localRotation) |  | 


## `ConsoleCommands`

```csharp
public class ThunderRoad.ConsoleCommands

```

Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AllowBloodEffects(`Boolean` active) |  | 
| `void` | DespawnAllItems() |  | 
| `void` | DespawnAllNPC() |  | 
| `void` | DespawnPlayer() |  | 
| `void` | EndWave() |  | 
| `String` | GetAvailableLevels() |  | 
| `String` | GetCreatureTable() |  | 
| `String` | GetDungeonRooms() |  | 
| `String` | GetDungeonSeed() |  | 
| `String` | GetGameVersion() |  | 
| `String` | GetItems() |  | 
| `void` | KillAll() |  | 
| `void` | LoadLevel(`String` levelId) |  | 
| `void` | LoadLevelMode(`String` levelId, `String` modeName) |  | 
| `void` | LoadLevelMode(`String` levelId, `String` modeName, `String[]` options) |  | 
| `void` | PerfRoomTest() |  | 
| `void` | PerfTest(`String` levelId) |  | 
| `void` | QuitGame() |  | 
| `void` | ReloadJsonAndAssets() |  | 
| `void` | ReloadLevel(`Boolean` useSameSeed) |  | 
| `void` | SetBitmask(`Int32` bitmask) |  | 
| `String` | SetComboButton(`ComboButton` comboButton) |  | 
| `void` | SetInfiniteArrows(`Boolean` active) |  | 
| `void` | SetInfiniteImbue(`Boolean` active) |  | 
| `void` | SetLightProbe(`Boolean` active) |  | 
| `String` | SetMonitorResolution(`Int32` width, `Int32` height, `Boolean` fullscreen = False) |  | 
| `void` | SetOculusMRC(`State` state) |  | 
| `void` | SetPlayerFaction(`Int32` factionId) |  | 
| `void` | SetPlayerVisibilityDistance(`Single` sightDistance) |  | 
| `void` | SetProbeVolume(`Boolean` active) |  | 
| `void` | SetTimeScale(`Single` scale) |  | 
| `void` | SpawnCreature(`String` creatureId) |  | 
| `void` | SpawnCreature(`String` creatureId, `Int32` factionId = 3, `String` containerID = null, `String` brainId = null) |  | 
| `void` | SpawnCreatureTable(`String` creatureTableId) |  | 
| `void` | SpawnItem(`String` itemId) |  | 
| `void` | StopPerfRoomTest() |  | 
| `void` | TeleportToRoom(`Int32` roomIndex) |  | 
| `void` | ToggleBookMenu() |  | 
| `void` | UnLoadLevel() |  | 
| `void` | UpdateLightVolume() |  | 


## `Container`

```csharp
public class ThunderRoad.Container
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | containerID |  | 
| `Boolean` | contentLoaded |  | 
| `List<Content>` | contents |  | 
| `Creature` | creature |  | 
| `LoadContent` | loadContent |  | 


Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `ContentChangeEvent` | OnContentAddEvent |  | 
| `ContentLoadedEvent` | OnContentLoadedEvent |  | 
| `ContentChangeEvent` | OnContentRemoveEvent |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Content` | AddContent(`ItemData` itemData, `List<SavedValue>` customValues = null) |  | 
| `void` | Awake() |  | 
| `List<ValueDropdownItem<String>>` | GetAllContainerID() |  | 
| `void` | Load() |  | 
| `void` | Load(`List<Content>` content) |  | 
| `void` | LoadAllPurchasable() |  | 
| `void` | LoadFromContainerId() |  | 
| `void` | LoadFromPlayerInventory() |  | 
| `void` | RemoveContent(`Content` content) |  | 
| `void` | Start() |  | 


## `ContainerData`

```csharp
public class ThunderRoad.ContainerData
    : CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Content>` | contents |  | 
| `String` | description |  | 
| `String` | displayName |  | 
| `List<String>` | generationOutput |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `CatalogData` | Clone() |  | 
| `List<Content>` | GetContents() |  | 
| `Int32` | GetCurrentVersion() |  | 
| `void` | OnCatalogRefresh() |  | 
| `void` | TestGeneration() |  | 


## `ContainerSpawner`

```csharp
public class ThunderRoad.ContainerSpawner
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | containerId |  | 
| `Boolean` | disallowDespawn |  | 
| `Boolean` | pooled |  | 
| `Boolean` | spawnOnStart |  | 
| `List<Transform>` | spawnPoints |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<ValueDropdownItem<String>>` | GetAllContainerId() |  | 
| `void` | OnItemSpawn(`Item` item) |  | 
| `void` | Spawn() |  | 
| `void` | Start() |  | 


## `Creature`

```csharp
public class ThunderRoad.Creature
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AsyncOperationHandle<GameObject>` | addressableHandle |  | 
| `KeyValuePair`2[]` | animationClipOverrides |  | 
| `Single` | animationDampTime |  | 
| `Animator` | animator |  | 
| `AnimatorOverrideController` | animatorOverrideController |  | 
| `Brain` | brain |  | 
| `Transform` | centerEyes |  | 
| `FeetClimber` | climber |  | 
| `Container` | container |  | 
| `String` | creatureId |  | 
| `CreatureSpawner` | creatureSpawner |  | 
| `Single` | cullingDetectionCycleSpeed |  | 
| `Single` | cullingDetectionCycleTime |  | 
| `Boolean` | cullingDetectionEnabled |  | 
| `Single` | currentHealth |  | 
| `Room` | currentRoom |  | 
| `CreatureData` | data |  | 
| `Action` | dynamicAnimationendEndCallback |  | 
| `AnimationClip` | dynamicEndReplaceClip |  | 
| `AnimationClip` | dynamicLoopReplaceClip |  | 
| `AnimationClip` | dynamicStartReplaceClip |  | 
| `Equipment` | equipment |  | 
| `Vector3` | eyeCameraOffset |  | 
| `Faction` | faction |  | 
| `Int32` | factionId |  | 
| `Single` | fallAliveAnimationHeight |  | 
| `Single` | fallAliveDestabilizeHeight |  | 
| `FallState` | fallState |  | 
| `RagdollFoot` | footLeft |  | 
| `RagdollFoot` | footRight |  | 
| `Single` | groundStabilizationLastTime |  | 
| `Single` | groundStabilizationMaxVelocity |  | 
| `Single` | groundStabilizationMinDuration |  | 
| `Single` | groundStabilizeDuration |  | 
| `RagdollHand` | handLeft |  | 
| `RagdollHand` | handRight |  | 
| `Single` | handToBodyRotationMaxAngle |  | 
| `Single` | handToBodyRotationMaxVelocity |  | 
| `Single` | headMaxAngle |  | 
| `Single` | headMinAngle |  | 
| `Boolean` | hidden |  | 
| `Single` | ikLocomotionAngularSpeedThreshold |  | 
| `Single` | ikLocomotionSpeedThreshold |  | 
| `Boolean` | initialized |  | 
| `Boolean` | isCulled |  | 
| `Boolean` | isKilled |  | 
| `Boolean` | isPlayer |  | 
| `Boolean` | isPlayingDynamicAnimation |  | 
| `Transform` | jaw |  | 
| `Vector3` | jawMaxRotation |  | 
| `CollisionInstance` | lastDamage |  | 
| `Single` | lastDamageTime |  | 
| `Creature` | lastInteractionCreature |  | 
| `Single` | lastInteractionTime |  | 
| `LightVolumeReceiver` | lightVolumeReceiver |  | 
| `Boolean` | loaded |  | 
| `Locomotion` | locomotion |  | 
| `LODGroup` | lodGroup |  | 
| `Mana` | mana |  | 
| `ManikinLocations` | manikinLocations |  | 
| `ManikinPartList` | manikinParts |  | 
| `ManikinProperties` | manikinProperties |  | 
| `Single` | maxHealth |  | 
| `Morphology` | morphology |  | 
| `JsonWardrobeLocations` | orgWardrobeLocations |  | 
| `Player` | player |  | 
| `Boolean` | pooled |  | 
| `Ragdoll` | ragdoll |  | 
| `List<RendererData>` | renderers |  | 
| `Single` | resurrectMinHeal |  | 
| `Single` | spawnTime |  | 
| `Single` | stationaryVelocityThreshold |  | 
| `Boolean` | stepEnabled |  | 
| `Vector3` | stepTargetPos |  | 
| `Single` | stepThreshold |  | 
| `Boolean` | toogleTPose |  | 
| `Single` | turnAnimSpeed |  | 
| `Boolean` | turnRelativeToHand |  | 
| `Single` | turnSpeed |  | 
| `Single` | turnTargetAngle |  | 
| `Boolean` | updateReveal |  | 
| `Renderer` | vfxRenderer |  | 
| `SpawnGroup` | waveSpawnGroup |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Locomotion` | currentLocomotion |  | 
| `State` | state |  | 


Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `DamageEvent` | OnDamageEvent |  | 
| `SimpleDelegate` | OnDataLoaded |  | 
| `DespawnEvent` | OnDespawnEvent |  | 
| `FallEvent` | OnFallEvent |  | 
| `HealEvent` | OnHealEvent |  | 
| `SimpleDelegate` | OnHeightChanged |  | 
| `KillEvent` | OnKillEvent |  | 
| `ResurrectEvent` | OnResurrectEvent |  | 
| `ZoneEvent` | OnZoneEvent |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | Damage(`CollisionInstance` collisionInstance) |  | 
| `void` | Despawn(`Single` delay) |  | 
| `void` | Despawn() |  | 
| `List<ValueDropdownItem<String>>` | GetAllCreatureID() |  | 
| `List<ValueDropdownItem<Int32>>` | GetAllFactionID() |  | 
| `Single` | GetAnimatorHeightRatio() |  | 
| `Color` | GetColor(`ColorModifier` colorModifier) |  | 
| `Single` | GetEyesHeight() |  | 
| `RagdollFoot` | GetFoot(`Side` side) |  | 
| `RagdollHand` | GetHand(`Side` side) |  | 
| `Single` | GetHeight() |  | 
| `Int32` | GetLODFromManikinGroupPart(`ManikinGroupPart` manikinGroupPart, `Renderer` renderer) |  | 
| `Renderer` | GetRendererForVFX() |  | 
| `Boolean` | HaveRendererData(`SkinnedMeshRenderer` skinnedMeshRenderer) |  | 
| `void` | Heal(`Single` heal, `Creature` healer) |  | 
| `void` | Hide(`Boolean` hide) |  | 
| `void` | Init() |  | 
| `void` | InitAnimatorHashs() |  | 
| `Boolean` | IsAnimatorBusy() |  | 
| `Boolean` | IsEnemy(`Creature` creatureTarget) |  | 
| `Boolean` | IsVisible() |  | 
| `void` | Kill() |  | 
| `void` | Kill(`CollisionInstance` collisionInstance) |  | 
| `void` | Load(`PlayerCharacterData` playerCharacterData = null) |  | 
| `void` | Load(`CreatureData` data, `PlayerCharacterData` playerCharacterData = null) |  | 
| `void` | OnDisable() |  | 
| `void` | OnEnable() |  | 
| `void` | OnEnterZone(`Zone` zone, `RagdollPart` ragdollPart) |  | 
| `void` | OnExitZone(`Zone` zone) |  | 
| `void` | OnManikinChangedEvent(`ManikinPart[]` partsAdded) |  | 
| `void` | PlayAnimation(`AnimationData` animationData, `Action` endCallback = null) |  | 
| `void` | PlayAnimation(`AnimationClip` animationClip, `Boolean` loop, `Single` speedMultiplier = 1, `Action` endCallback = null) |  | 
| `void` | PlayAnimation(`AnimationClip` startAnimationClip, `AnimationClip` loopAnimationClip, `AnimationClip` endAnimationClip, `Single` speedMultiplier = 1, `Action` endCallback = null) |  | 
| `void` | RefreshCollisionOfGrabbedItems() |  | 
| `void` | RefreshFallState(`FallState` newState, `Boolean` force = False) |  | 
| `void` | RefreshMorphology() |  | 
| `void` | RefreshRenderers() |  | 
| `void` | Resurrect(`Single` newHealth, `Creature` resurrector) |  | 
| `void` | SetAnimatorBusy(`Boolean` active) |  | 
| `void` | SetAnimatorHeightRatio(`Single` height) |  | 
| `void` | SetColor(`Color` color, `ColorModifier` colorModifier, `Boolean` updateProperties = False) |  | 
| `void` | SetCull(`Boolean` cull) |  | 
| `void` | SetFaction(`Int32` factionId) |  | 
| `void` | SetGrabbedObjectLayer(`LayerName` layerName) |  | 
| `void` | SetHeight(`CreatureData` creatureData) |  | 
| `void` | SetHeight(`Single` height) |  | 
| `Boolean` | ShouldUpdateWhenOffscreen(`RendererData` rendererData) |  | 
| `void` | Start() |  | 
| `void` | StopAnimation(`Boolean` interrupt = False) |  | 
| `void` | StopShock() |  | 
| `void` | Teleport(`Vector3` position, `Quaternion` rotation) |  | 
| `void` | TestDamage() |  | 
| `void` | TestKill() |  | 
| `void` | ToogleTPose() |  | 
| `void` | TryElectrocute(`Single` power, `Single` duration, `Boolean` forced, `Boolean` imbueHit, `EffectData` effectData = null) |  | 
| `Boolean` | TryGetManikinProperty(`String` name, `ManikinProperty&` manikinProperty) |  | 
| `void` | TryPush(`PushType` type, `Vector3` direction, `Int32` pushLevel, `Type` bodyPart = 0) |  | 
| `void` | Update() |  | 
| `void` | UpdateDynamicAnimation() |  | 
| `void` | UpdateFall() |  | 
| `void` | UpdateRenderers() |  | 
| `void` | UpdateReveal() |  | 
| `void` | UpdateStep(`Vector3` position, `Single` stepSpeedMultiplier = 1, `Single` stepThresholdMultiplier = 1) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Creature>` | all |  | 
| `List<Creature>` | allActive |  | 
| `Int32` | hashDynamicInterrupt |  | 
| `Int32` | hashDynamicLoop |  | 
| `Int32` | hashDynamicLoop3 |  | 
| `Int32` | hashDynamicOneShot |  | 
| `Int32` | hashDynamicSpeedMultiplier |  | 
| `Int32` | hashFalling |  | 
| `Int32` | hashFeminity |  | 
| `Int32` | hashGetUp |  | 
| `Int32` | hashHeight |  | 
| `Boolean` | hashInitialized |  | 
| `Int32` | hashIsBusy |  | 
| `Int32` | hashSpeed |  | 
| `Int32` | hashStaticIdle |  | 
| `Int32` | hashStrafe |  | 
| `Int32` | hashTstance |  | 
| `Int32` | hashTurn |  | 
| `Boolean` | meshRaycast |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | CompareByLastInteractionTime(`Creature` c1, `Creature` c2) |  | 


## `CreatureData`

```csharp
public class ThunderRoad.CreatureData
    : CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | adjustHeightToPlayer |  | 
| `Single` | adjustHeightToPlayerDelta |  | 
| `Int32` | androidPooledCount |  | 
| `Int32` | avoidancePriority |  | 
| `Int32` | baseXP |  | 
| `String` | brainId |  | 
| `Single` | climbingForceMaxPosition |  | 
| `Single` | climbingForceMaxRotation |  | 
| `Vector2` | climbingForcePositionSpringDamperMult |  | 
| `String` | closeHandPoseId |  | 
| `String` | containerID |  | 
| `HandPoseData` | defaultCloseHandPoseData |  | 
| `HandPoseData` | defaultOpenHandPoseData |  | 
| `String` | displayName |  | 
| `ExpressionData` | expressionAngryData |  | 
| `String` | expressionAngryId |  | 
| `ExpressionData` | expressionAttackData |  | 
| `String` | expressionAttackId |  | 
| `ExpressionData` | expressionChokeData |  | 
| `String` | expressionChokeId |  | 
| `ExpressionData` | expressionDeathData |  | 
| `String` | expressionDeathId |  | 
| `ExpressionData` | expressionPainData |  | 
| `String` | expressionPainId |  | 
| `List<EyeColor>` | eyesColors |  | 
| `Int32` | factionId |  | 
| `Single` | focus |  | 
| `Single` | focusRegen |  | 
| `Single` | forceMaxPosition |  | 
| `Single` | forceMaxRotation |  | 
| `Vector2` | forcePositionSpringDamper |  | 
| `Vector2` | forcePositionSpringDamper2HMult |  | 
| `Vector2` | forceRotationSpringDamper |  | 
| `Vector2` | forceRotationSpringDamper2HMult |  | 
| `Vector2` | forceSpringDamper2HNoDomMult |  | 
| `Gender` | gender |  | 
| `Single` | gripForceMaxPosition |  | 
| `Single` | gripForceMaxRotation |  | 
| `Vector2` | gripForcePositionSpringDamperMult |  | 
| `Vector2` | gripForceRotationSpringDamperMult |  | 
| `List<HairColor>` | hairColors |  | 
| `Int16` | health |  | 
| `Single` | jumpClimbVerticalMaxVelocityRatio |  | 
| `EffectData` | jumpEffectData |  | 
| `String` | jumpEffectId |  | 
| `Single` | locomotionAirSpeed |  | 
| `Single` | locomotionBackwardSpeedMult |  | 
| `Single` | locomotionFlyDrag |  | 
| `Single` | locomotionGroundDrag |  | 
| `Single` | locomotionJumpClimbHorizontalMultiplier |  | 
| `Single` | locomotionJumpClimbVerticalMultiplier |  | 
| `Single` | locomotionJumpForce |  | 
| `Single` | locomotionJumpMaxDuration |  | 
| `Single` | locomotionMass |  | 
| `Single` | locomotionRunSpeedMult |  | 
| `Single` | locomotionSpeed |  | 
| `Single` | locomotionStrafeSpeedMult |  | 
| `Single` | mana |  | 
| `Single` | manaRegen |  | 
| `String` | name |  | 
| `String` | openHandPoseId |  | 
| `LayerMask` | overlapMask |  | 
| `Single` | overlapMinDelay |  | 
| `Single` | overlapRadius |  | 
| `AnimationCurve` | playerFallDamageCurve |  | 
| `EffectData` | playerFallDamageEffectData |  | 
| `String` | playerFallDamageEffectId |  | 
| `Int32` | pooledCount |  | 
| `PossesionScaling` | possesionScaling |  | 
| `String` | prefabAddress |  | 
| `IResourceLocation` | prefabLocation |  | 
| `RagdollData` | ragdollData |  | 
| `Single` | randomMaxHeight |  | 
| `Single` | randomMinHeight |  | 
| `Boolean` | removeMeshWhenPooled |  | 
| `List<Color>` | skinColors |  | 
| `List<String>` | voices |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ConfigCreature(`Creature` creature, `WayPoint[]` waypoints = null) |  | 
| `List<ValueDropdownItem<String>>` | GetAllBrainID() |  | 
| `List<ValueDropdownItem<String>>` | GetAllContainerID() |  | 
| `List<ValueDropdownItem<String>>` | GetAllDamagerID() |  | 
| `List<ValueDropdownItem<String>>` | GetAllEffectID() |  | 
| `List<ValueDropdownItem<String>>` | GetAllExpressionId() |  | 
| `List<ValueDropdownItem<Int32>>` | GetAllFactionID() |  | 
| `List<ValueDropdownItem<String>>` | GetAllHandPoseId() |  | 
| `List<ValueDropdownItem<String>>` | GetAllItemID() |  | 
| `List<ValueDropdownItem<String>>` | GetAllSpellID() |  | 
| `List<ValueDropdownItem<String>>` | GetAllVoiceID() |  | 
| `Int32` | GetCurrentVersion() |  | 
| `Int32` | GetPooledCount() |  | 
| `void` | InstantiateAsync(`Vector3` position, `Quaternion` rotation, `Transform` parent, `Action<Creature>` callback = null) |  | 
| `IEnumerator` | InstantiateCoroutine(`Vector3` position, `Quaternion` rotation, `Transform` parent, `Action<Creature>` result) |  | 
| `void` | OnCatalogRefresh() |  | 
| `IEnumerator` | OnCatalogRefreshCoroutine() |  | 
| `EyeColor` | PickEyesColor() |  | 
| `HairColor` | PickHairColor() |  | 
| `Color` | PickSkinColor() |  | 
| `void` | SpawnAsync(`Vector3` position, `Quaternion` rotation, `Transform` parent = null, `Boolean` pooled = True, `WayPoint[]` waypoints = null, `Action<Creature>` callback = null) |  | 
| `IEnumerator` | SpawnCoroutine(`Vector3` position, `Quaternion` rotation, `Transform` parent, `Action<Creature>` result, `Boolean` pooled = True, `WayPoint[]` waypoints = null) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | creatureIndex |  | 
| `Int32` | index |  | 
| `Transform` | poolRoot |  | 
| `List<Pool>` | pools |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ClearPool() |  | 
| `void` | CreatureInstantiateCallback(`Creature` creature, `Pool` pool) |  | 
| `void` | DespawnAllPooled() |  | 
| `IEnumerator` | GeneratePool() |  | 
| `void` | ReturnToPool(`Creature` creature) |  | 


## `CreatureSpawner`

```csharp
public class ThunderRoad.CreatureSpawner
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | creatureTableID |  | 
| `Boolean` | ignoreRoomMaxNPC |  | 
| `UnityEvent` | OnAlertState |  | 
| `CreatureEvent` | OnCombatState |  | 
| `UnityEvent` | OnDespawn |  | 
| `UnityEvent` | OnKill |  | 
| `Boolean` | pooled |  | 
| `Boolean` | spawnAtRandomWaypoint |  | 
| `List<SpawnedCreature>` | spawnedCreatures |  | 
| `Boolean` | spawning |  | 
| `Boolean` | spawnOnNavMesh |  | 
| `Boolean` | spawnOnStart |  | 
| `Transform` | waypointsRoot |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<ValueDropdownItem<String>>` | GetAllCreatureTableID() |  | 
| `void` | OnDrawGizmos() |  | 
| `void` | Spawn() |  | 
| `void` | Start() |  | 


## `CreatureTable`

```csharp
public class ThunderRoad.CreatureTable
    : CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | description |  | 
| `List<Drop>` | drops |  | 
| `String` | generationBrain |  | 
| `String` | generationContainer |  | 
| `String` | generationCreature |  | 
| `String` | generationFaction |  | 
| `Boolean` | linkedToGenderRatio |  | 
| `Vector2Int` | minMaxDifficulty |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CalculateWeight(`Int32` difficulty) |  | 
| `CatalogData` | Clone() |  | 
| `void` | CopyFromLeft() |  | 
| `void` | CopyFromRight() |  | 
| `void` | EditorCalculateWeight() |  | 
| `Int32` | GetCurrentVersion() |  | 
| `void` | OnCatalogRefresh() |  | 
| `void` | TestGeneration() |  | 
| `Boolean` | TryPick(`CreatureData&` creatureData) |  | 
| `Boolean` | TryPick(`Int32` difficulty, `CreatureData&` creatureData) |  | 
| `Boolean` | TryPick(`Int32` difficulty, `Int32` pickCount, `CreatureData&` creatureData) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Difficulty` | showWeightDifficulty |  | 


## `CustomReference`

```csharp
public class ThunderRoad.CustomReference

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | name |  | 
| `Transform` | transform |  | 


## `DamageModifierData`

```csharp
public class ThunderRoad.DamageModifierData
    : CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Collision>` | collisions |  | 
| `DamageType` | damageType |  | 
| `Modifier` | defaultModifier |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | GetCurrentVersion() |  | 
| `Modifier` | GetModifier(`CollisionInstance` collisionInstance) |  | 
| `void` | OnCatalogRefresh() |  | 


## `Damager`

```csharp
public class ThunderRoad.Damager
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `ColliderGroup` | colliderGroup |  | 
| `Collider` | colliderOnly |  | 
| `CollisionHandler` | collisionHandler |  | 
| `Damager` | damagerImbue |  | 
| `DamagerData` | data |  | 
| `Direction` | direction |  | 
| `Collider` | dmgCollider |  | 
| `Collider` | lastHitCollider |  | 
| `Single` | lastHitTime |  | 
| `RagdollPart` | lastSliceRagdollPart |  | 
| `Single` | lastSliceTime |  | 
| `Boolean` | loaded |  | 
| `Single` | penetrationDepth |  | 
| `Boolean` | penetrationExitOnMaxDepth |  | 
| `Single` | penetrationLength |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `Boolean` | CheckAngles(`Vector3` vector, `Vector3` normal) |  | 
| `Boolean` | CheckAngles(`Vector3` vector) |  | 
| `Boolean` | CheckPenetration(`CollisionInstance` collisionInstance) |  | 
| `Boolean` | CheckSlice(`Vector3` contactPoint, `RagdollPart` ragdollPart) |  | 
| `List<ValueDropdownItem<String>>` | GetAllEffectID() |  | 
| `void` | GetColliderOnlyFromThis() |  | 
| `Vector3` | GetMaxDepthPosition(`Boolean` reverted) |  | 
| `Boolean` | InsideColliderGroup(`ColliderGroup` targetColliderGroup, `Vector3` point) |  | 
| `void` | Load(`DamagerData` damagerData, `CollisionHandler` collisionHandler) |  | 
| `void` | OnDrawGizmosSelected() |  | 
| `void` | OnGrab(`Handle` handle, `RagdollHand` ragdollHand) |  | 
| `void` | OnRelease(`Handle` handle, `RagdollHand` ragdollHand, `Boolean` throwing) |  | 
| `void` | OnSnap(`Holder` holder) |  | 
| `void` | Penetrate(`CollisionInstance` collisionInstance, `Boolean` usePressure) |  | 
| `void` | RefreshJointDrive(`CollisionInstance` collisionInstance) |  | 
| `void` | RefreshPushLevel(`CollisionInstance` collisionInstance) |  | 
| `Boolean` | TryHit(`CollisionInstance` collisionInstance) |  | 
| `Boolean` | TryHitByPressure(`CollisionInstance` collisionInstance) |  | 
| `void` | UnPenetrate(`CollisionInstance` collisionInstance) |  | 
| `void` | UnPenetrateAll() |  | 
| `void` | UpdatePenetration(`CollisionInstance` collisionInstance) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | dismembermentEnabled |  | 


## `DamagerData`

```csharp
public class ThunderRoad.DamagerData
    : CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | addForce |  | 
| `Single` | addForceDuration |  | 
| `ForceMode` | addForceMode |  | 
| `Boolean` | addForceNormalize |  | 
| `Single` | addForceRagdollOtherMultiplier |  | 
| `Single` | addForceRagdollPartMultiplier |  | 
| `Single` | addForceSlowMoMultiplier |  | 
| `ObjectState` | addForceState |  | 
| `TargetType` | addForceTargetType |  | 
| `Boolean` | badAngleBluntFallback |  | 
| `Single` | badAngleDamage |  | 
| `String` | badAngleMaterialDamageId |  | 
| `DamageModifierData` | badAngleModifierData |  | 
| `Single` | badAngleRecoilMultiplier |  | 
| `DamageModifierData` | damageModifierData |  | 
| `String` | damageModifierId |  | 
| `Boolean` | dismembermentAllowed |  | 
| `Single` | dismembermentMinVelocity |  | 
| `Single` | dismembermentNoPenetrationDuration |  | 
| `Single` | dyingAnimationMaxVelocity |  | 
| `Single` | hitDelayByCollider |  | 
| `Single` | intensityMaxVelocity |  | 
| `Single` | intensityMinVelocity |  | 
| `Single` | minSelfVelocity |  | 
| `Boolean` | penetrationAllowed |  | 
| `Boolean` | penetrationAllowSlide |  | 
| `Single` | penetrationDamage |  | 
| `Single` | penetrationDamper |  | 
| `Single` | penetrationDeepDepthMultiplier |  | 
| `Boolean` | penetrationEffect |  | 
| `Single` | penetrationHeldDamperIn |  | 
| `Single` | penetrationHeldDamperOut |  | 
| `Single` | penetrationInitialVelocityMultiplier |  | 
| `Boolean` | penetrationPressureAllowed |  | 
| `AnimationCurve` | penetrationPressureForceCurve |  | 
| `Single` | penetrationPressureMaxDot |  | 
| `Single` | penetrationShortDepth |  | 
| `Single` | penetrationShortDepthAngle |  | 
| `Single` | penetrationSkewerDamage |  | 
| `Boolean` | penetrationSkewerDetection |  | 
| `Single` | penetrationSlideDamper |  | 
| `PenetrationTempModifier` | penetrationTempModifier |  | 
| `Single` | penetrationTempModifierDamperIn |  | 
| `Single` | penetrationTempModifierDamperOut |  | 
| `Single` | penetrationTempModifierDuration |  | 
| `Single` | playerDamageMultiplier |  | 
| `Single` | playerMaxDamage |  | 
| `Single` | playerMinDamage |  | 
| `Boolean` | selfDamage |  | 
| `AnimationCurve` | staticVelocityDamageCurve |  | 
| `Single` | throwedMultiplier |  | 
| `Tier[]` | tiers |  | 
| `AnimationCurve` | velocityDamageCurve |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<ValueDropdownItem<String>>` | GetAllDamagerModifierID() |  | 
| `List<ValueDropdownItem<String>>` | GetAllMaterialID() |  | 
| `Int32` | GetCurrentVersion() |  | 
| `Tier` | GetTier(`CollisionHandler` collisionHandler) |  | 
| `Tier` | GetTier(`Int32` tier) |  | 
| `void` | OnCatalogRefresh() |  | 


## `DamageStruct`

```csharp
public struct ThunderRoad.DamageStruct

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | active |  | 
| `Boolean` | badAngle |  | 
| `Single` | baseDamage |  | 
| `Single` | damage |  | 
| `Damager` | damager |  | 
| `DamageType` | damageType |  | 
| `Boolean` | hasPenetrationEffect |  | 
| `Item` | hitItem |  | 
| `RagdollPart` | hitRagdollPart |  | 
| `Single` | lastDepth |  | 
| `Single` | lastRumbleDepth |  | 
| `Modifier` | materialModifier |  | 
| `Penetration` | penetration |  | 
| `Single` | penetrationCutAxisPos |  | 
| `EffectInstance` | penetrationDeepEffectInstance |  | 
| `Boolean` | penetrationDeepReached |  | 
| `Single` | penetrationDepth |  | 
| `Single` | penetrationDepthReached |  | 
| `EffectInstance` | penetrationEffectInstance |  | 
| `Single` | penetrationEffectLastDistance |  | 
| `Boolean` | penetrationFromThrow |  | 
| `ConfigurableJoint` | penetrationJoint |  | 
| `Transform` | penetrationPoint |  | 
| `Rigidbody` | penetrationRb |  | 
| `Boolean` | penetrationTempRb |  | 
| `Int32` | pushLevel |  | 
| `Boolean` | stickMassModified |  | 
| `Single` | time |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Reset(`Boolean` exceptPreDamage = False) |  | 


## `DamageType`

```csharp
public enum ThunderRoad.DamageType
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | Unknown |  | 
| `1` | Pierce |  | 
| `2` | Slash |  | 
| `3` | Blunt |  | 
| `4` | Energy |  | 


## `DataManager`

```csharp
public class ThunderRoad.DataManager
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `DataSource` | dataSource |  | 
| `Boolean` | editorLoadAddressableBundles |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<AsyncOperationHandle<IResourceLocator>>` | handles |  | 
| `DataManager` | local |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DeleteCharacter(`String` id) |  | 
| `void` | DeleteLocalFile(`String` fileName) |  | 
| `List<PlayerCharacterData>` | GetCharacters() |  | 
| `List<String>` | GetLocalFiles(`String` searchPattern = *.*) |  | 
| `String` | GetLocalMyGamesPath(`String` folderName) |  | 
| `String` | GetLocalSavePath() |  | 
| `String` | GetLocalScreenshotPath() |  | 
| `IEnumerator` | LoadAddressableAssets() |  | 
| `void` | LoadDLL() |  | 
| `T` | LoadLocalFile(`String` fileName) |  | 
| `void` | OverrideCharacters() |  | 
| `void` | OverrideOptions() |  | 
| `String` | SaveCharacter(`PlayerCharacterData` characterData) |  | 
| `void` | SaveLocalFile(`Object` obj, `String` fileName) |  | 


## `DebugTool`

```csharp
public class ThunderRoad.DebugTool
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | autoRotate |  | 
| `Single` | autoRotateSpeed |  | 
| `Boolean` | autoSetPlayerInvincibleAndStartWave |  | 
| `String` | equipItemID |  | 
| `Int32` | playerFaction |  | 
| `String` | wave |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AutoTurnHand() |  | 
| `Scores` | CheckScores() |  | 
| `void` | CreatureAllPlayAnimation(`Boolean` active) |  | 
| `void` | DespawnItems() |  | 
| `void` | DespawnNPC() |  | 
| `void` | DespawnPlayer() |  | 
| `void` | DropItem() |  | 
| `void` | EquipItem(`String` itemID) |  | 
| `void` | EquipItemCallback(`Item` item) |  | 
| `List<ValueDropdownItem<Int32>>` | GetAllFactionID() |  | 
| `List<ValueDropdownItem<String>>` | GetAllItemID() |  | 
| `List<ValueDropdownItem<String>>` | GetAllWaveID() |  | 
| `void` | SetNPCAnimRbActive(`Boolean` active) |  | 
| `void` | SetNPCAnimRbDetectCollisions(`Boolean` active) |  | 
| `void` | SetNPCBodyDetectCollisions(`Boolean` active) |  | 
| `void` | SetNPCBodyRbActive(`Boolean` active, `Boolean` ignoreHand) |  | 
| `void` | SetNPCColliders(`Boolean` active) |  | 
| `void` | SetNPCSolverIteration(`Int32` solverIterations) |  | 
| `void` | SetNPCSolverVelocityIterations(`Int32` solverVelocityIterations) |  | 
| `void` | SetNPCState(`State` state) |  | 
| `void` | SetPlayerFaction() |  | 
| `void` | StartWave() |  | 
| `void` | StopWave() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Coroutine` | perfRoomTestCoroutine |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CheckLightMapMode() |  | 
| `void` | DropWeaponsNPC() |  | 
| `void` | KillRandomNPC() |  | 
| `void` | LightProbesTetrahedralize() |  | 
| `void` | LoadLevel(`String` levelId) |  | 
| `void` | PerfRoomTest() |  | 
| `void` | SetGameViewRenderMode(`GameViewRenderMode` gameViewRenderMode) |  | 
| `void` | SetPlayerVisibilityDistance(`Single` sightDistance) |  | 
| `void` | SetRenderScale(`Single` scale = 1) |  | 
| `void` | SliceAllParts() |  | 
| `void` | SliceHeadAll() |  | 
| `void` | SliceRandomNPCHead() |  | 
| `void` | SliceRandomNPCLeftArm() |  | 
| `void` | SliceRandomNPCLeftFoot() |  | 
| `void` | SliceRandomNPCLeftHand() |  | 
| `void` | SliceRandomNPCLeftLeg() |  | 
| `void` | SliceRandomNPCNeck() |  | 
| `void` | SliceRandomNPCRightArm() |  | 
| `void` | SliceRandomNPCRightFoot() |  | 
| `void` | SliceRandomNPCRightHand() |  | 
| `void` | SliceRandomNPCRightLeg() |  | 
| `void` | StopPerfRoomTest() |  | 
| `void` | TeleportPlayerToRoom(`Int32` roomIndex) |  | 
| `void` | ToggleMenuBook() |  | 
| `void` | UnLoadLevel() |  | 


## `DeepCopyByExpressionTrees`

```csharp
public static class ThunderRoad.DeepCopyByExpressionTrees

```

Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `T` | DeepCopyByExpressionTree(this `T` original, `Dictionary<Object, Object>` copiedReferencesDict = null) |  | 


## `DisableOnCondition`

```csharp
public class ThunderRoad.DisableOnCondition
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Condition` | condition |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnEnable() |  | 


## `DisableOnPlatform`

```csharp
public class ThunderRoad.DisableOnPlatform
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | allowStrip |  | 
| `Platform` | platform |  | 
| `PlatformFilter` | platformFilter |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `Boolean` | ConcernPlatform(`Platform` platform) |  | 


## `DisplayText`

```csharp
public class ThunderRoad.DisplayText
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `RectTransform` | canvas |  | 
| `RawImage` | image |  | 
| `Transform` | panelToFade |  | 
| `Text` | textHalf |  | 
| `Text` | textLarge |  | 
| `VideoPlayer` | videoPlayer |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Hide() |  | 
| `void` | ShowTextTest() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `DisplayText` | instance |  | 
| `Boolean` | shown |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ShowText(`TextPriority` aTextPriority) |  | 
| `void` | StopText() |  | 


## `DoorTransition`

```csharp
public class ThunderRoad.DoorTransition
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `HingeJoint` | doorJoint |  | 
| `Single` | fadeoutTimer |  | 
| `List<Collider>` | ignoredColliders |  | 
| `Single` | jointSensitivity |  | 
| `String` | mapDestination |  | 
| `Transform` | teleportDestination |  | 


## `Dungeon`

```csharp
public class ThunderRoad.Dungeon
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | cullingEnabled |  | 
| `String` | dungeonFlowAddress |  | 
| `RuntimeDungeon` | dungeonGenerator |  | 
| `UnityNavMeshAdapter` | dungeonNavMeshAdapter |  | 
| `Boolean` | initialized |  | 
| `Transform` | playerTransform |  | 
| `Boolean` | proxyOnly |  | 
| `Int32` | roomInitCount |  | 
| `List<Room>` | rooms |  | 
| `Int32` | seed |  | 
| `Int32` | startingRoomIndex |  | 
| `Boolean` | staticBatchRooms |  | 
| `Boolean` | useRandomSeed |  | 


Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `DungeonGeneratedEvent` | onDungeonGenerated |  | 
| `PlayerChangeRoomEvent` | onPlayerChangeRoom |  | 
| `RoomVisibilityChangeEvent` | onRoomVisibilityChange |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DespawnAllCreatures() |  | 
| `void` | DespawnAllItems() |  | 
| `void` | GenerateDungeon() |  | 
| `void` | GenerateGlobalNavMesh() |  | 
| `void` | GenerateNavMesh() |  | 
| `void` | Init() |  | 
| `void` | InvokeRoomVisibilityChange(`Room` room) |  | 
| `void` | OnAllRoomInitialized() |  | 
| `void` | OnPlayerChangeRoom(`Room` oldRoom, `Room` newRoom) |  | 
| `void` | OnRoomInitialized(`Room` roomInitialized) |  | 
| `void` | RefreshCulling() |  | 
| `Room` | SearchRoomFromPosition(`Vector3` position, `Room` fromRoom = null) |  | 
| `void` | SetCulling(`Boolean` enabled) |  | 
| `IEnumerator` | SpawnRoomsCoroutine() |  | 
| `void` | ToggleCulling() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `DungeonDoor` | playerNearEntryDoor |  | 
| `DungeonDoor` | playerNearExitDoor |  | 
| `Room` | playerRoom |  | 


## `DungeonDoor`

```csharp
public class ThunderRoad.DungeonDoor
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `DungeonDoor` | connectedDoor |  | 
| `Room` | connectedRoom |  | 
| `Doorway` | doorway |  | 
| `Single` | fadeAudioMinDistanceRatio |  | 
| `Single` | fadeMaxDistance |  | 
| `Single` | fadeRoomMinDistanceRatio |  | 
| `MaterialPropertyBlock` | fakeInteriorBlock |  | 
| `FRI` | fri |  | 
| `Bounds` | localBounds |  | 
| `UnityEvent` | onAwakeIfEntry |  | 
| `UnityEvent` | onAwakeIfExit |  | 
| `DungeonDoor` | oppositeDoor |  | 
| `Room` | room |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Bounds` | worldBounds |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Init() |  | 
| `void` | OnAllRoomInitialized() |  | 
| `void` | OnPlayerChangeRoom(`Room` oldRoom, `Room` newRoom) |  | 
| `void` | OnPlayerEnter() |  | 
| `void` | OnPlayerExit() |  | 
| `void` | SetFakeDoorOpacity(`Single` fade) |  | 
| `void` | SlowUpdate() |  | 


## `Duplicator`

```csharp
public class ThunderRoad.Duplicator
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector2Int` | quantity |  | 
| `GameObject` | source |  | 
| `Vector2` | spacing |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Clean() |  | 
| `void` | Duplicate() |  | 


## `DynamicText`

```csharp
public class ThunderRoad.DynamicText
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Info` | info |  | 
| `Single` | updateRate |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | SetTextState(`Boolean` state) |  | 
| `void` | SetTextState(`Int32` value) |  | 
| `void` | SetTextState(`Single` value) |  | 
| `void` | SetTextState(`String` stringValue) |  | 
| `void` | UpdateCaption() |  | 


## `Effect`

```csharp
public class ThunderRoad.Effect
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `DespawnCallback` | despawnCallback |  | 
| `Boolean` | isOutOfPool |  | 
| `Boolean` | isPooled |  | 
| `EffectModule` | module |  | 
| `Step` | step |  | 
| `Int32` | stepCustomHashId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CollisionStay(`Vector3` position, `Quaternion` rotation, `Single` speed) |  | 
| `void` | CollisionStay(`Vector3` position, `Quaternion` rotation, `Single` speed, `Single` intensity) |  | 
| `void` | CollisionStay(`Single` speed) |  | 
| `void` | CollisionStay(`Single` speed, `Single` intensity) |  | 
| `void` | Despawn() |  | 
| `void` | End(`Boolean` loopOnly = False) |  | 
| `void` | InvokeDespawnCallback() |  | 
| `void` | Play() |  | 
| `void` | SetCollider(`Collider` collider) |  | 
| `void` | SetIntensity(`Single` value, `Boolean` loopOnly = False) |  | 
| `void` | SetMainGradient(`Gradient` gradient) |  | 
| `void` | SetMesh(`Mesh` mesh) |  | 
| `void` | SetNoise(`Boolean` noise) |  | 
| `void` | SetRenderer(`Renderer` renderer, `Boolean` secondary) |  | 
| `void` | SetSecondaryGradient(`Gradient` gradient) |  | 
| `void` | SetSize(`Single` value) |  | 
| `void` | SetSource(`Transform` transform) |  | 
| `void` | SetSpeed(`Single` value, `Boolean` loopOnly = False) |  | 
| `void` | SetTarget(`Transform` transform) |  | 
| `void` | Stop() |  | 


## `EffectAudio`

```csharp
public class ThunderRoad.EffectAudio
    : Effect

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioContainer` | audioContainer |  | 
| `AudioSource` | audioSource |  | 
| `Boolean` | doNoise |  | 
| `EffectLink` | effectLink |  | 
| `Single` | globalPitch |  | 
| `Single` | globalVolumeDb |  | 
| `Boolean` | hasNoise |  | 
| `AnimationCurve` | highPassCutoffFrequencyCurve |  | 
| `AudioHighPassFilter` | highPassFilter |  | 
| `AnimationCurve` | highPassResonanceQCurve |  | 
| `Single` | loopFadeDelay |  | 
| `AnimationCurve` | lowPassCutoffFrequencyCurve |  | 
| `AudioLowPassFilter` | lowPassFilter |  | 
| `AnimationCurve` | lowPassResonanceQCurve |  | 
| `Noise` | noise |  | 
| `AnimationCurve` | pitchCurve |  | 
| `EffectLink` | pitchEffectLink |  | 
| `Single` | playDelay |  | 
| `Single` | playTime |  | 
| `Single` | randomMaxTime |  | 
| `Single` | randomMinTime |  | 
| `Boolean` | randomPitch |  | 
| `Boolean` | randomPlay |  | 
| `AnimationCurve` | reverbDryLevelCurve |  | 
| `AudioReverbFilter` | reverbFilter |  | 
| `SteamAudioSource` | steamAudioSource |  | 
| `Boolean` | useHighPassFilter |  | 
| `Boolean` | useLowPassFilter |  | 
| `Boolean` | useReverbFilter |  | 
| `AnimationCurve` | volumeCurve |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `IEnumerator` | AudioFadeOut() |  | 
| `void` | Despawn() |  | 
| `void` | End(`Boolean` loopOnly = False) |  | 
| `void` | Play() |  | 
| `void` | RandomPlay() |  | 
| `void` | SetIntensity(`Single` value, `Boolean` loopOnly = False) |  | 
| `void` | SetNoise(`Boolean` noise) |  | 
| `void` | SetSpeed(`Single` value, `Boolean` loopOnly = False) |  | 
| `void` | SetVariation(`Single` value, `Boolean` loopOnly = False) |  | 
| `void` | Stop() |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | DecibelToLinear(`Single` dB) |  | 
| `Single` | LinearToDecibel(`Single` linear) |  | 


## `EffectBundle`

```csharp
public class ThunderRoad.EffectBundle

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `EffectData` | effectData |  | 
| `String` | effectId |  | 
| `List<String>` | ignoredEffects |  | 
| `Type[]` | ignoredEffectTypes |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `EffectBundle` | Clone() |  | 
| `List<ValueDropdownItem<String>>` | GetAllEffectID() |  | 
| `List<ValueDropdownItem<String>>` | GetAllEffetModuleTypes() |  | 
| `void` | OnCatalogRefresh() |  | 


## `EffectData`

```csharp
public class ThunderRoad.EffectData
    : CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `EffectGroupData` | effectGroupData |  | 
| `String` | groupId |  | 
| `List<EffectGroupData>` | groupParents |  | 
| `List<EffectModule>` | modules |  | 
| `Single` | volumeDb |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<ValueDropdownItem<String>>` | GetAllEffectGroupID() |  | 
| `void` | OnCatalogRefresh() |  | 
| `IEnumerator` | OnCatalogRefreshCoroutine() |  | 
| `void` | RefreshGroupParents() |  | 
| `EffectInstance` | Spawn(`Transform` parent, `Boolean` pooled = True, `Type[]` ignoredEffectModules) |  | 
| `EffectInstance` | Spawn(`Vector3` position, `Quaternion` rotation, `Transform` parent = null, `CollisionInstance` collisionInstance = null, `Boolean` pooled = True, `Type[]` ignoredEffectModules) |  | 


## `EffectDecal`

```csharp
public class ThunderRoad.EffectDecal
    : Effect

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Gradient` | baseColorGradient |  | 
| `Single` | baseLifeTime |  | 
| `Gradient` | emissionColorGradient |  | 
| `Single` | emissionLifeTime |  | 
| `Single` | fadeRefreshSpeed |  | 
| `EffectTarget` | linkBaseColor |  | 
| `EffectTarget` | linkEmissionColor |  | 
| `MaterialPropertyBlock` | materialPropertyBlock |  | 
| `MeshRenderer` | meshRenderer |  | 
| `Single` | playTime |  | 
| `Vector3` | size |  | 
| `AnimationCurve` | sizeCurve |  | 
| `Single` | sizeRandomRange |  | 
| `Boolean` | useSizeCurve |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CollisionStay(`Vector3` position, `Quaternion` rotation, `Single` intensity) |  | 
| `void` | Despawn() |  | 
| `void` | End(`Boolean` loopOnly = False) |  | 
| `void` | Play() |  | 
| `void` | SetIntensity(`Single` value, `Boolean` loopOnly = False) |  | 
| `void` | SetMainGradient(`Gradient` gradient) |  | 
| `void` | SetSecondaryGradient(`Gradient` gradient) |  | 
| `void` | Stop() |  | 
| `void` | UpdateLifeTime() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | colorPropertyID |  | 
| `Mesh` | defaultCubeMesh |  | 
| `Int32` | emissionPropertyID |  | 


## `EffectGroupData`

```csharp
public class ThunderRoad.EffectGroupData
    : CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | globalMaxPitch |  | 
| `Single` | globalMinPitch |  | 
| `Single` | globalVolumeDb |  | 
| `String` | groupId |  | 
| `EffectGroupData` | parentGroupData |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<ValueDropdownItem<String>>` | GetAllEffectGroupID() |  | 
| `String` | GetPath(`String` path = ) |  | 
| `void` | OnCatalogRefresh() |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<EffectGroupData>` | GetGroupParents(`EffectGroupData` effectGroupData) |  | 


## `EffectInstance`

```csharp
public class ThunderRoad.EffectInstance

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Effect>` | effects |  | 
| `Boolean` | isPlaying |  | 


Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `EffectFinishEvent` | onEffectFinished |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddEffect(`EffectData` effectData, `Vector3` position, `Quaternion` rotation, `Single` intensity = 0, `Single` speed = 0, `Transform` parent = null, `CollisionInstance` collisionInstance = null, `Boolean` pooled = True, `Type[]` ignoredEffectModules) |  | 
| `void` | CollisionStay(`Vector3` position, `Quaternion` rotation, `Single` speed) |  | 
| `void` | CollisionStay(`Vector3` position, `Quaternion` rotation, `Single` speed, `Single` intensity) |  | 
| `void` | CollisionStay(`Single` speed) |  | 
| `void` | CollisionStay(`Single` speed, `Single` intensity) |  | 
| `void` | Despawn() |  | 
| `void` | End(`Boolean` loopOnly = False, `Single` endIntensity = -1) |  | 
| `Boolean` | IsIgnoredModule(`EffectModule` effectModule, `Type[]` ignoredEffectModules) |  | 
| `void` | OnEffectDespawn(`Effect` effect) |  | 
| `void` | Play(`Int32` stepCustomHashId = 0) |  | 
| `void` | SetCollider(`Collider` collider) |  | 
| `void` | SetIntensity(`Single` value) |  | 
| `void` | SetLayer(`Int32` layer) |  | 
| `void` | SetMainGradient(`Gradient` gradient) |  | 
| `void` | SetMesh(`Mesh` mesh) |  | 
| `void` | SetNoise(`Boolean` noise) |  | 
| `void` | SetParent(`Transform` parent) |  | 
| `void` | SetRenderer(`Renderer` renderer, `Boolean` secondary) |  | 
| `void` | SetSecondaryGradient(`Gradient` gradient) |  | 
| `void` | SetSource(`Transform` transform) |  | 
| `void` | SetSpeed(`Single` value) |  | 
| `void` | SetTarget(`Transform` transform) |  | 
| `void` | Stop(`Int32` stepCustomHashId = 0) |  | 


## `EffectLink`

```csharp
public enum ThunderRoad.EffectLink
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | Intensity |  | 
| `1` | Speed |  | 


## `EffectMesh`

```csharp
public class ThunderRoad.EffectMesh
    : Effect

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Gradient` | currentMainGradient |  | 
| `Gradient` | currentSecondaryGradient |  | 
| `Single` | currentValue |  | 
| `AnimationCurve` | curveMeshrotY |  | 
| `AnimationCurve` | curveMeshSize |  | 
| `AnimationCurve` | intensityCurve |  | 
| `Single` | lifeTime |  | 
| `EffectTarget` | linkBaseColor |  | 
| `EffectTarget` | linkEmissionColor |  | 
| `EffectTarget` | linkTintColor |  | 
| `MaterialPropertyBlock` | materialPropertyBlock |  | 
| `MeshFilter` | meshFilter |  | 
| `MeshRenderer` | meshRenderer |  | 
| `Vector3` | meshRotation |  | 
| `Coroutine` | meshRotationFadeCoroutine |  | 
| `Single` | meshRotationFadeDuration |  | 
| `Boolean` | meshRotationFading |  | 
| `Boolean` | meshRotationFromIntensity |  | 
| `Vector3` | meshSize |  | 
| `Coroutine` | meshSizeFadeCoroutine |  | 
| `Single` | meshSizeFadeDuration |  | 
| `Boolean` | meshSizeFading |  | 
| `Boolean` | meshSizeFromIntensity |  | 
| `Single` | playTime |  | 
| `Int32` | poolCount |  | 
| `Single` | refreshSpeed |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Despawn() |  | 
| `void` | End(`Boolean` loopOnly = False) |  | 
| `void` | Play() |  | 
| `void` | SetIntensity(`Single` value, `Boolean` loopOnly = False) |  | 
| `void` | SetMainGradient(`Gradient` gradient) |  | 
| `void` | SetSecondaryGradient(`Gradient` gradient) |  | 
| `void` | Stop() |  | 
| `void` | UpdateLifeTime() |  | 


## `EffectModule`

```csharp
public class ThunderRoad.EffectModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `FilterLogic` | colliderGroupFilterLogic |  | 
| `Int32[]` | colliderGroupHashes |  | 
| `String[]` | colliderGroupsFilter |  | 
| `Int32[]` | damagerHashes |  | 
| `String[]` | damagersFilter |  | 
| `FilterLogic` | damagersFilterLogic |  | 
| `DamagerFilter` | damagerStateFilter |  | 
| `DamageTypeFilter` | damageTypeFilter |  | 
| `Int32[]` | imbueHashes |  | 
| `String[]` | imbuesFilter |  | 
| `FilterLogic` | imbuesFilterLogic |  | 
| `Boolean` | isGore |  | 
| `PenetrationFilter` | penetrationFilter |  | 
| `PlateformFilter` | plateformFilter |  | 
| `Step` | step |  | 
| `String` | stepCustomId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CheckPlateform() |  | 
| `void` | Clean() |  | 
| `void` | CopyHDRToNonHDR() |  | 
| `T` | EditorLoad(`String` address) |  | 
| `List<ValueDropdownItem<String>>` | GetAllColliderGroupID() |  | 
| `List<ValueDropdownItem<String>>` | GetAllDamagerID() |  | 
| `List<ValueDropdownItem<String>>` | GetAllSpellCastChargeID() |  | 
| `void` | OnCatalogRefresh(`EffectData` effectData, `Boolean` editorLoad = False) |  | 
| `IEnumerator` | RefreshCoroutine(`EffectData` effectData, `Boolean` editorLoad = False) |  | 
| `Boolean` | Spawn(`EffectData` effectData, `Vector3` position, `Quaternion` rotation, `Effect&` effect, `Single` intensity = 0, `Single` speed = 0, `Transform` parent = null, `CollisionInstance` collisionInstance = null, `Boolean` pooled = True) |  | 


## `EffectModuleAudio`

```csharp
public class ThunderRoad.EffectModuleAudio
    : EffectModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioContainer` | audioContainer |  | 
| `String` | audioContainerAddress |  | 
| `AudioMixerName` | audioMixer |  | 
| `Single` | cullMinVolume |  | 
| `Single` | dopplerLevel |  | 
| `EffectLink` | effectLink |  | 
| `AnimationCurve` | highPassCutoffFrequencyCurve |  | 
| `AnimationCurve` | highPassResonanceQCurve |  | 
| `Boolean` | isNoiseForAI |  | 
| `Single` | loopFadeDelay |  | 
| `AnimationCurve` | lowPassCutoffFrequencyCurve |  | 
| `AnimationCurve` | lowPassResonanceQCurve |  | 
| `Single` | maxDistance |  | 
| `Single` | minDistance |  | 
| `AnimationCurve` | pitchCurve |  | 
| `EffectLink` | pitchEffectLink |  | 
| `Single` | playDelay |  | 
| `Single` | randomMaxTime |  | 
| `Single` | randomMinTime |  | 
| `Boolean` | randomPitch |  | 
| `Boolean` | randomPlay |  | 
| `AnimationCurve` | reverbDryLevelCurve |  | 
| `Single` | spatialBlend |  | 
| `Boolean` | useHighPassFilter |  | 
| `Boolean` | useLowPassFilter |  | 
| `Boolean` | useReverbFilter |  | 
| `AnimationCurve` | volumeCurve |  | 
| `Single` | volumeDb |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Clean() |  | 
| `EffectAudio` | Configure(`EffectAudio` effectAudio, `EffectData` effectData, `Single` globalVolume, `Single` globalPitch) |  | 
| `IEnumerator` | RefreshCoroutine(`EffectData` effectData, `Boolean` editorLoad = False) |  | 
| `Boolean` | Spawn(`EffectData` effectData, `Vector3` position, `Quaternion` rotation, `Effect&` effect, `Single` intensity = 1, `Single` speed = 1, `Transform` parent = null, `CollisionInstance` collisionInstance = null, `Boolean` pooled = True) |  | 
| `void` | UpdateVolumeCurveToDb() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<EffectAudio>` | pool |  | 
| `Transform` | poolRoot |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ClearPool() |  | 
| `void` | Despawn(`EffectAudio` effect) |  | 
| `void` | DespawnAllPooled() |  | 
| `void` | GeneratePool() |  | 
| `void` | SetSteamAudio(`Boolean` active) |  | 


## `EffectModuleDecal`

```csharp
public class ThunderRoad.EffectModuleDecal
    : EffectModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | allowRagdollPart |  | 
| `Single` | baseLifeTime |  | 
| `Single` | emissionLifeTime |  | 
| `Single` | fadeRefreshSpeed |  | 
| `EffectTarget` | linkBaseColor |  | 
| `EffectTarget` | linkEmissionColor |  | 
| `Color` | mainColorEnd |  | 
| `Color` | mainColorStart |  | 
| `Color` | mainNoHdrColorEnd |  | 
| `Color` | mainNoHdrColorStart |  | 
| `Material` | material |  | 
| `String` | materialAddress |  | 
| `Int32` | priority |  | 
| `Color` | secondaryColorEnd |  | 
| `Color` | secondaryColorStart |  | 
| `Color` | secondaryNoHdrColorEnd |  | 
| `Color` | secondaryNoHdrColorStart |  | 
| `Vector3` | size |  | 
| `AnimationCurve` | sizeCurve |  | 
| `Single` | sizeRandomRange |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Gradient` | MainGradient |  | 
| `Gradient` | MainGradientNoHdr |  | 
| `Gradient` | SecondaryGradient |  | 
| `Gradient` | SecondaryGradientNoHdr |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Clean() |  | 
| `EffectDecal` | Configure(`EffectDecal` effectDecal, `EffectData` effectData) |  | 
| `void` | CopyHDRToNonHDR() |  | 
| `void` | OnCatalogRefresh(`EffectData` effectData, `Boolean` editorLoad = False) |  | 
| `IEnumerator` | RefreshCoroutine(`EffectData` effectData, `Boolean` editorLoad = False) |  | 
| `Boolean` | Spawn(`EffectData` effectData, `Vector3` position, `Quaternion` rotation, `Effect&` effect, `Single` intensity = 0, `Single` speed = 0, `Transform` parent = null, `CollisionInstance` collisionInstance = null, `Boolean` pooled = True) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<EffectDecal>` | pool |  | 
| `Int32` | poolCount |  | 
| `Transform` | poolRoot |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ClearPool() |  | 
| `void` | Despawn(`EffectDecal` effectDecal) |  | 
| `void` | DespawnAllPooled() |  | 
| `void` | GeneratePool() |  | 


## `EffectModuleMesh`

```csharp
public class ThunderRoad.EffectModuleMesh
    : EffectModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AnimationCurve` | intensityCurve |  | 
| `Single` | lifeTime |  | 
| `EffectTarget` | linkBaseColor |  | 
| `EffectTarget` | linkEmissionColor |  | 
| `EffectTarget` | linkTintColor |  | 
| `Vector3` | localRotation |  | 
| `Vector3` | localScale |  | 
| `Color` | mainColorEnd |  | 
| `Color` | mainColorStart |  | 
| `Color` | mainNoHdrColorEnd |  | 
| `Color` | mainNoHdrColorStart |  | 
| `List<MaterialProperty>` | materialProperties |  | 
| `List<Materials>` | materials |  | 
| `Mesh` | mesh |  | 
| `String` | meshAddress |  | 
| `Single` | refreshSpeed |  | 
| `Single` | rotationFadeDuration |  | 
| `AnimationCurve` | rotationYCurve |  | 
| `Color` | secondaryColorEnd |  | 
| `Color` | secondaryColorStart |  | 
| `Color` | secondaryNoHdrColorEnd |  | 
| `Color` | secondaryNoHdrColorStart |  | 
| `AnimationCurve` | sizeCurve |  | 
| `Single` | sizeFadeDuration |  | 
| `Boolean` | useRotationYCurve |  | 
| `Boolean` | useSizeCurve |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Gradient` | MainGradient |  | 
| `Gradient` | MainGradientNoHdr |  | 
| `Gradient` | SecondaryGradient |  | 
| `Gradient` | SecondaryGradientNoHdr |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Clean() |  | 
| `EffectMesh` | Configure(`EffectMesh` effect, `EffectData` effectData) |  | 
| `void` | CopyHDRToNonHDR() |  | 
| `void` | OnCatalogRefresh(`EffectData` effectData, `Boolean` editorLoad = False) |  | 
| `IEnumerator` | RefreshCoroutine(`EffectData` effectData, `Boolean` editorLoad = False) |  | 
| `Boolean` | Spawn(`EffectData` effectData, `Vector3` position, `Quaternion` rotation, `Effect&` effect, `Single` intensity = 0, `Single` speed = 0, `Transform` parent = null, `CollisionInstance` collisionInstance = null, `Boolean` pooled = True) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<EffectMesh>` | pool |  | 
| `Transform` | poolRoot |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ClearPool() |  | 
| `void` | Despawn(`EffectMesh` effect) |  | 
| `void` | DespawnAllPooled() |  | 
| `void` | GeneratePool() |  | 


## `EffectModuleParticle`

```csharp
public class ThunderRoad.EffectModuleParticle
    : EffectModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `EffectData` | collisionEffectData |  | 
| `String` | collisionEffectId |  | 
| `Single` | collisionEmitRate |  | 
| `LayerMask` | collisionLayerMask |  | 
| `Single` | collisionMaxGroundAngle |  | 
| `Single` | collisionMaxIntensity |  | 
| `Single` | collisionMinIntensity |  | 
| `Boolean` | collisionUseMainGradient |  | 
| `Boolean` | collisionUseSecondaryGradient |  | 
| `EffectLink` | effectLink |  | 
| `String` | effectParticleAddress |  | 
| `EffectParticle` | effectParticlePrefab |  | 
| `Boolean` | goreParticle |  | 
| `AnimationCurve` | intensityCurve |  | 
| `Vector3` | localScale |  | 
| `Color` | mainColorEnd |  | 
| `Color` | mainColorStart |  | 
| `Color` | mainNoHdrColorEnd |  | 
| `Color` | mainNoHdrColorStart |  | 
| `Boolean` | renderInLateUpdate |  | 
| `AnimationCurve` | scaleCurve |  | 
| `Color` | secondaryColorEnd |  | 
| `Color` | secondaryColorStart |  | 
| `Color` | secondaryNoHdrColorEnd |  | 
| `Color` | secondaryNoHdrColorStart |  | 
| `Boolean` | useScaleCurve |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Gradient` | MainGradient |  | 
| `Gradient` | MainGradientNoHdr |  | 
| `Gradient` | SecondaryGradient |  | 
| `Gradient` | SecondaryGradientNoHdr |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Clean() |  | 
| `EffectParticle` | Configure(`EffectParticle` effectParticle, `EffectData` effectData) |  | 
| `void` | CopyHDRToNonHDR() |  | 
| `List<ValueDropdownItem<String>>` | GetAllEffectID() |  | 
| `void` | OnCatalogRefresh(`EffectData` effectData, `Boolean` editorLoad = False) |  | 
| `IEnumerator` | RefreshCoroutine(`EffectData` effectData, `Boolean` editorLoad = False) |  | 
| `Boolean` | Spawn(`EffectData` effectData, `Vector3` position, `Quaternion` rotation, `Effect&` effect, `Single` intensity = 0, `Single` speed = 0, `Transform` parent = null, `CollisionInstance` collisionInstance = null, `Boolean` pooled = True) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Dictionary<EffectParticle, List<EffectParticle>>` | pool |  | 
| `Transform` | poolRoot |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ClearPool() |  | 
| `void` | Despawn(`EffectParticle` effectParticle) |  | 
| `void` | DespawnAllPooled() |  | 
| `void` | GeneratePool() |  | 


## `EffectModuleReveal`

```csharp
public class ThunderRoad.EffectModuleReveal
    : EffectModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | allowItem |  | 
| `Boolean` | allowRagdollPart |  | 
| `Direction` | applyOn |  | 
| `Single` | depth |  | 
| `Texture` | maskTexture |  | 
| `String` | maskTextureAddress |  | 
| `Vector4` | maxChannelMultiplier |  | 
| `Single` | maxSize |  | 
| `Vector4` | minChannelMultiplier |  | 
| `Single` | minSize |  | 
| `Single` | offsetDistance |  | 
| `Vector4` | penetrationChannelMultiplier |  | 
| `Single` | penetrationSize |  | 
| `RevealData[]` | revealData |  | 
| `TypeFilter` | typeFilter |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `EffectReveal` | Configure(`EffectReveal` effect, `EffectData` effectData, `CollisionInstance` collisionInstance, `CollisionHandler` targetCollisionHandler) |  | 
| `IEnumerator` | RefreshCoroutine(`EffectData` effectData, `Boolean` editorLoad = False) |  | 
| `Boolean` | Spawn(`EffectData` effectData, `Vector3` position, `Quaternion` rotation, `Effect&` effect, `Single` intensity = 0, `Single` speed = 0, `Transform` parent = null, `CollisionInstance` collisionInstance = null, `Boolean` pooled = True) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<EffectReveal>` | pool |  | 
| `Transform` | poolRoot |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ClearPool() |  | 
| `void` | Despawn(`EffectReveal` effect) |  | 
| `void` | DespawnAllPooled() |  | 
| `void` | GeneratePool() |  | 


## `EffectModuleShader`

```csharp
public class ThunderRoad.EffectModuleShader
    : EffectModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | lifeTime |  | 
| `EffectTarget` | linkBaseColor |  | 
| `EffectTarget` | linkEmissionColor |  | 
| `Color` | mainColorEnd |  | 
| `Color` | mainColorStart |  | 
| `Color` | mainNoHdrColorEnd |  | 
| `Color` | mainNoHdrColorStart |  | 
| `Single` | refreshSpeed |  | 
| `Color` | secondaryColorEnd |  | 
| `Color` | secondaryColorStart |  | 
| `Color` | secondaryNoHdrColorEnd |  | 
| `Color` | secondaryNoHdrColorStart |  | 
| `Boolean` | useSecondaryRenderer |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Gradient` | MainGradient |  | 
| `Gradient` | MainGradientNoHdr |  | 
| `Gradient` | SecondaryGradient |  | 
| `Gradient` | SecondaryGradientNoHdr |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Clean() |  | 
| `EffectShader` | Configure(`EffectShader` effect, `EffectData` effectData) |  | 
| `void` | CopyHDRToNonHDR() |  | 
| `void` | OnCatalogRefresh(`EffectData` effectData, `Boolean` editorLoad = False) |  | 
| `Boolean` | Spawn(`EffectData` effectData, `Vector3` position, `Quaternion` rotation, `Effect&` effect, `Single` intensity = 0, `Single` speed = 0, `Transform` parent = null, `CollisionInstance` collisionInstance = null, `Boolean` pooled = True) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<EffectShader>` | pool |  | 
| `Transform` | poolRoot |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ClearPool() |  | 
| `void` | Despawn(`EffectShader` effect) |  | 
| `void` | DespawnAllPooled() |  | 
| `void` | GeneratePool() |  | 


## `EffectModuleVfx`

```csharp
public class ThunderRoad.EffectModuleVfx
    : EffectModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AnimationCurve` | intensityCurve |  | 
| `Single` | lifeTime |  | 
| `Vector3` | localScale |  | 
| `Boolean` | lookAtTarget |  | 
| `Color` | mainColorEnd |  | 
| `Color` | mainColorStart |  | 
| `Color` | mainNoHdrColorEnd |  | 
| `Color` | mainNoHdrColorStart |  | 
| `List<VfxProperty>` | materialProperties |  | 
| `String` | meshAddress |  | 
| `Mesh` | meshAsset |  | 
| `MeshBakeMode` | pointCacheBakeMode |  | 
| `Distribution` | pointCacheDistribution |  | 
| `Int32` | pointCacheMapSize |  | 
| `Int32` | pointCachePointCount |  | 
| `Int32` | pointCacheSeed |  | 
| `Boolean` | pointCacheSkinnedMeshUpdate |  | 
| `AnimationCurve` | scaleCurve |  | 
| `Color` | secondaryColorEnd |  | 
| `Color` | secondaryColorStart |  | 
| `Color` | secondaryNoHdrColorEnd |  | 
| `Color` | secondaryNoHdrColorStart |  | 
| `Boolean` | useMesh |  | 
| `Boolean` | usePointCache |  | 
| `Boolean` | useScaleCurve |  | 
| `Boolean` | useSecondaryRenderer |  | 
| `String` | vfxAddress |  | 
| `VisualEffectAsset` | vfxAsset |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Gradient` | MainGradient |  | 
| `Gradient` | MainGradientNoHdr |  | 
| `Gradient` | SecondaryGradient |  | 
| `Gradient` | SecondaryGradientNoHdr |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Clean() |  | 
| `EffectVfx` | Configure(`EffectVfx` effectVfx, `EffectData` effectData) |  | 
| `void` | CopyHDRToNonHDR() |  | 
| `void` | OnCatalogRefresh(`EffectData` effectData, `Boolean` editorLoad = False) |  | 
| `IEnumerator` | RefreshCoroutine(`EffectData` effectData, `Boolean` editorLoad = False) |  | 
| `Boolean` | Spawn(`EffectData` effectData, `Vector3` position, `Quaternion` rotation, `Effect&` effect, `Single` intensity = 0, `Single` speed = 0, `Transform` parent = null, `CollisionInstance` collisionInstance = null, `Boolean` pooled = True) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<EffectVfx>` | pool |  | 
| `Transform` | poolRoot |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ClearPool() |  | 
| `void` | Despawn(`EffectVfx` effect) |  | 
| `void` | DespawnAllPooled() |  | 
| `void` | GeneratePool() |  | 


## `EffectParticle`

```csharp
public class ThunderRoad.EffectParticle
    : Effect

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<EffectParticleChild>` | childs |  | 
| `Gradient` | currentMainGradient |  | 
| `Gradient` | currentSecondaryGradient |  | 
| `Single` | currentValue |  | 
| `EffectLink` | effectLink |  | 
| `AnimationCurve` | intensityCurve |  | 
| `Single` | lifeTime |  | 
| `MaterialPropertyBlock` | materialPropertyBlock |  | 
| `MinMaxCurve` | minMaxCurve |  | 
| `Single` | playTime |  | 
| `Int32` | poolCount |  | 
| `Boolean` | renderInLateUpdate |  | 
| `ParticleSystem` | rootParticleSystem |  | 
| `AnimationCurve` | scaleCurve |  | 
| `Boolean` | useScaleCurve |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Despawn() |  | 
| `void` | End(`Boolean` loopOnly = False) |  | 
| `void` | LateUpdate() |  | 
| `void` | Play() |  | 
| `void` | SetCollider(`Collider` collider) |  | 
| `void` | SetIntensity(`Single` value, `Boolean` loopOnly = False) |  | 
| `void` | SetMainGradient(`Gradient` gradient) |  | 
| `void` | SetMesh(`Mesh` mesh) |  | 
| `void` | SetRenderer(`Renderer` renderer, `Boolean` secondary) |  | 
| `void` | SetSecondaryGradient(`Gradient` gradient) |  | 
| `void` | SetSpeed(`Single` value, `Boolean` loopOnly = False) |  | 
| `void` | SetVariation(`Single` value, `Boolean` loopOnly = False) |  | 
| `void` | Stop() |  | 


## `EffectParticleChild`

```csharp
public class ThunderRoad.EffectParticleChild
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | burst |  | 
| `Boolean` | collider |  | 
| `AnimationCurve` | curveBurst |  | 
| `AnimationCurve` | curveDuration |  | 
| `AnimationCurve` | curveLifeTime |  | 
| `AnimationCurve` | curveLightIntensity |  | 
| `AnimationCurve` | curveRate |  | 
| `AnimationCurve` | curveShapeArc |  | 
| `AnimationCurve` | curveShapeRadius |  | 
| `AnimationCurve` | curveSize |  | 
| `AnimationCurve` | curveSpeed |  | 
| `AnimationCurve` | curvevelocityOverLifetime |  | 
| `Boolean` | duration |  | 
| `Boolean` | emitEffectOnCollision |  | 
| `Boolean` | ignoreAlpha |  | 
| `Boolean` | lifeTime |  | 
| `Boolean` | lightIntensity |  | 
| `EffectTarget` | linkBaseColor |  | 
| `EffectTarget` | linkEmissionColor |  | 
| `EffectTarget` | linkStartColor |  | 
| `EffectTarget` | linkStartGradient |  | 
| `EffectTarget` | linkTintColor |  | 
| `MaterialPropertyBlock` | materialPropertyBlock |  | 
| `Boolean` | mesh |  | 
| `ParticleCollisionSpawner` | particleCollisionSpawner |  | 
| `ParticleSystemRenderer` | particleRenderer |  | 
| `ParticleSystem` | particleSystem |  | 
| `Int16` | randomRangeBurst |  | 
| `Single` | randomRangeLifeTime |  | 
| `Single` | randomRangeRate |  | 
| `Single` | randomRangeSize |  | 
| `Single` | randomRangeSpeed |  | 
| `Boolean` | rate |  | 
| `Boolean` | shapeArc |  | 
| `Boolean` | shapeRadius |  | 
| `Boolean` | size |  | 
| `Boolean` | speed |  | 
| `EffectTarget` | useRenderer |  | 
| `Boolean` | velocityOverLifetime |  | 


## `EffectReveal`

```csharp
public class ThunderRoad.EffectReveal
    : Effect

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Direction` | applyOn |  | 
| `CollisionHandler` | collisionHandler |  | 
| `Vector4` | currentChannelMultiplier |  | 
| `Single` | currentSize |  | 
| `Single` | depth |  | 
| `Texture` | maskTexture |  | 
| `Vector4` | maxChannelMultiplier |  | 
| `Single` | maxSize |  | 
| `Vector4` | minChannelMultiplier |  | 
| `Single` | minSize |  | 
| `Single` | offsetDistance |  | 
| `Single` | playTime |  | 
| `RevealData[]` | revealData |  | 
| `List<RevealMaterialController>` | revealMaterialControllers |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Despawn() |  | 
| `void` | End(`Boolean` loopOnly = False) |  | 
| `void` | OnProjectCompleted(`Single` overTime) |  | 
| `void` | Play() |  | 
| `void` | SetIntensity(`Single` value, `Boolean` loopOnly = False) |  | 
| `void` | Stop() |  | 


## `EffectShader`

```csharp
public class ThunderRoad.EffectShader
    : Effect

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Gradient` | currentMainGradient |  | 
| `Gradient` | currentSecondaryGradient |  | 
| `Single` | currentValue |  | 
| `Single` | lifeTime |  | 
| `EffectTarget` | linkBaseColor |  | 
| `EffectTarget` | linkEmissionColor |  | 
| `MaterialInstance` | materialInstance |  | 
| `Single` | playTime |  | 
| `Single` | refreshSpeed |  | 
| `Boolean` | useSecondaryRenderer |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Despawn() |  | 
| `void` | End(`Boolean` loopOnly = False) |  | 
| `void` | Play() |  | 
| `void` | SetIntensity(`Single` value, `Boolean` loopOnly = False) |  | 
| `void` | SetMainGradient(`Gradient` gradient) |  | 
| `void` | SetRenderer(`Renderer` renderer, `Boolean` secondary) |  | 
| `void` | SetSecondaryGradient(`Gradient` gradient) |  | 
| `void` | Stop() |  | 
| `void` | UpdateLifeTime() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | colorPropertyID |  | 
| `Int32` | emissionPropertyID |  | 


## `EffectSpawner`

```csharp
public class ThunderRoad.EffectSpawner
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | autoIntensity |  | 
| `Collider` | collider |  | 
| `Boolean` | editorLoad |  | 
| `String` | effectId |  | 
| `EffectInstance` | effectInstance |  | 
| `Single` | intensity |  | 
| `AnimationCurve` | intensityCurve |  | 
| `Gradient` | mainGradient |  | 
| `Renderer` | mainRenderer |  | 
| `Mesh` | mesh |  | 
| `Single` | playTime |  | 
| `Gradient` | secondaryGradient |  | 
| `Renderer` | secondaryRenderer |  | 
| `Transform` | source |  | 
| `Boolean` | spawnOnStart |  | 
| `Single` | speed |  | 
| `Transform` | target |  | 
| `Boolean` | useMainGradient |  | 
| `Boolean` | useSecondaryGradient |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<ValueDropdownItem<String>>` | GetAllEffectID() |  | 
| `void` | Spawn() |  | 
| `IEnumerator` | SpawnCoroutine(`EffectData` effectData) |  | 
| `void` | Start() |  | 
| `void` | Stop() |  | 
| `void` | Update() |  | 


## `EffectTarget`

```csharp
public enum ThunderRoad.EffectTarget
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | None |  | 
| `1` | Main |  | 
| `2` | Secondary |  | 


## `EffectVfx`

```csharp
public class ThunderRoad.EffectVfx
    : Effect

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AnimationCurve` | curveEmitSize |  | 
| `Boolean` | emitSize |  | 
| `Boolean` | hasSource |  | 
| `Boolean` | hasTarget |  | 
| `AnimationCurve` | intensityCurve |  | 
| `Single` | lifeTime |  | 
| `Boolean` | lookAtTarget |  | 
| `PCache` | pCache |  | 
| `Single` | playTime |  | 
| `MeshBakeMode` | pointCacheBakeMode |  | 
| `Distribution` | pointCacheDistribution |  | 
| `Int32` | pointCacheMapSize |  | 
| `Int32` | pointCachePointCount |  | 
| `Int32` | pointCacheSeed |  | 
| `SkinnedMeshRenderer` | pointCacheSkinnedMeshRenderer |  | 
| `Boolean` | pointCacheSkinnedMeshUpdate |  | 
| `AnimationCurve` | scaleCurve |  | 
| `Transform` | sourceTransform |  | 
| `Int32` | srcPositionAngles |  | 
| `Int32` | srcPositionId |  | 
| `Int32` | srcPositionScale |  | 
| `Boolean` | stopping |  | 
| `Transform` | targetTransform |  | 
| `Int32` | tgtPositionAngles |  | 
| `Int32` | tgtPositionId |  | 
| `Int32` | tgtPositionScale |  | 
| `Boolean` | usePointCache |  | 
| `Boolean` | useScaleCurve |  | 
| `Boolean` | useSecondaryRenderer |  | 
| `VisualEffect` | vfx |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Despawn() |  | 
| `void` | End(`Boolean` loopOnly = False) |  | 
| `void` | LateUpdate() |  | 
| `void` | Play() |  | 
| `void` | SetCollider(`Collider` collider) |  | 
| `void` | SetIntensity(`Single` value, `Boolean` loopOnly = False) |  | 
| `void` | SetMainGradient(`Gradient` gradient) |  | 
| `void` | SetMesh(`Mesh` mesh) |  | 
| `void` | SetRenderer(`Renderer` renderer, `Boolean` secondary) |  | 
| `void` | SetSecondaryGradient(`Gradient` gradient) |  | 
| `void` | SetSource(`Transform` source) |  | 
| `void` | SetTarget(`Transform` target) |  | 
| `void` | Stop() |  | 
| `void` | Update() |  | 
| `void` | UpdateSource() |  | 
| `void` | UpdateTarget() |  | 


## `Equipment`

```csharp
public class ThunderRoad.Equipment
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Creature` | creature |  | 
| `Boolean` | equipWardrobesOnLoad |  | 
| `Boolean` | equipWeaponsOnLoad |  | 
| `List<Holder>` | holders |  | 
| `Int32` | spawningItemCount |  | 
| `Int32` | totalApparels |  | 
| `Int32` | totalTierApparels |  | 
| `Int32` | totalTierShields |  | 
| `Int32` | totalTierWeapons |  | 
| `Coroutine` | waitPartUpdateCoroutine |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | EquipAllWardrobes(`Boolean` bodyOnly, `Boolean` unequipAllWardrobes = True) |  | 
| `void` | EquipItem(`Content` contentItem, `Holder` holder) |  | 
| `void` | EquipWardrobe(`Content` content, `Boolean` updateParts = True) |  | 
| `void` | EquipWeapons() |  | 
| `Holder` | GetFirstFreeHolder(`String` slot = null, `Holder` ignoreHolder = null) |  | 
| `Holder` | GetFreeDrawHolder(`Side` side, `Boolean` hipsIsPriority, `String` slot = null, `Holder` ignoreHolder = null) |  | 
| `Handle` | GetHeldHandle(`Side` handSide) |  | 
| `Item` | GetHeldItem(`Side` handSide) |  | 
| `Item` | GetHeldWeapon(`Side` handSide) |  | 
| `Holder` | GetHolder(`DrawSlot` drawSlot) |  | 
| `Holder` | GetHolster(`String` name) |  | 
| `List<Item>` | GetHolsterWeapons() |  | 
| `Int32` | GetPendingApparelLoading() |  | 
| `Holder` | GetQuiverArrow() |  | 
| `Content` | GetWornContent(`String` channel, `Int32` layer) |  | 
| `Content` | GetWornContentLowerLayer(`String` channel, `String[]` onlyLayers) |  | 
| `void` | Init(`Creature` creature) |  | 
| `void` | Load() |  | 
| `void` | OnContainerContentRemoved(`Content` content) |  | 
| `void` | OnDespawn() |  | 
| `void` | OnUpdatePartCompleted(`ManikinPart[]` partsAdded) |  | 
| `void` | UnequipAllWardrobes(`Boolean` updateParts = False) |  | 
| `void` | UnequipWardrobe(`Content` content, `Boolean` updateParts = True) |  | 
| `void` | UnequipWeapons() |  | 
| `void` | UpdateParts() |  | 
| `IEnumerator` | WaitPartUpdateCoroutine() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | wornCustomVariableName |  | 


## `EventController`

```csharp
public class ThunderRoad.EventController
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | beginOnStart |  | 
| `ConcurentInvokeBehaviour` | concurentInvokeBehaviour |  | 
| `Coroutine` | coroutine |  | 
| `Int32` | invokeCount |  | 
| `Boolean[]` | invokedIndex |  | 
| `Int32` | invokeMaxIndex |  | 
| `Single` | loopCount |  | 
| `Single` | maxDelay |  | 
| `Int32` | maxInvoke |  | 
| `Single` | minDelay |  | 
| `UnityEvent` | timedEvent |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | Invoke() |  | 
| `void` | Invoke(`Int32` index) |  | 
| `void` | InvokeNow() |  | 
| `void` | Start() |  | 
| `void` | StopInvoke(`Int32` index) |  | 
| `void` | StopInvoke() |  | 


## `EventLoadLevel`

```csharp
public class ThunderRoad.EventLoadLevel
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | fadeInDuration |  | 
| `String` | levelId |  | 
| `List<LevelOption>` | levelOptions |  | 
| `String` | modeName |  | 
| `SaveOptions` | saveOptions |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | LoadLevel() |  | 
| `void` | LoadLevel(`String` levelId) |  | 
| `void` | LoadLevelNow() |  | 


## `EventManager`

```csharp
public class ThunderRoad.EventManager
    : MonoBehaviour

```

Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | InvokeCreatureHeal(`Creature` creature, `Single` heal, `Creature` healer) |  | 
| `void` | InvokeCreatureHit(`Creature` creature, `CollisionInstance` collisionInstance) |  | 
| `void` | InvokeCreatureKill(`Creature` creature, `Player` player, `CollisionInstance` collisionInstance, `EventTime` eventTime) |  | 
| `void` | InvokeCreatureParry(`Creature` creature, `CollisionInstance` collisionInstance) |  | 
| `void` | InvokeCreatureSpawn(`Creature` creature) |  | 
| `void` | InvokeDebugOptionChanged(`Parameter` parameter) |  | 
| `void` | InvokeDeflect(`Creature` source, `Item` item, `Creature` target) |  | 
| `void` | InvokeGameLoaded() |  | 
| `void` | InvokeLevelLoad(`LevelData` levelData, `EventTime` eventTime) |  | 
| `void` | InvokeLevelUnload(`LevelData` levelData, `EventTime` eventTime) |  | 
| `void` | InvokePlayerExposureChangeEvent(`Exposure` oldExposure, `Exposure` newExposure) |  | 
| `void` | InvokePossession(`Creature` newBody, `EventTime` eventTime) |  | 
| `void` | InvokeReloadJson(`EventTime` eventTime) |  | 
| `void` | InvokeUnpossession(`Creature` oldBody, `EventTime` eventTime) |  | 


Static Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `CreatureHealEvent` | onCreatureHeal |  | 
| `CreatureHitEvent` | onCreatureHit |  | 
| `CreatureKillEvent` | onCreatureKill |  | 
| `CreatureHitEvent` | onCreatureParry |  | 
| `CreatureSpawnedEvent` | onCreatureSpawn |  | 
| `DebugOptionChangedEvent` | onDebugOptionChange |  | 
| `DeflectEvent` | onDeflect |  | 
| `DefaultEvent` | onGameLoad |  | 
| `LevelLoadEvent` | onLevelLoad |  | 
| `LevelLoadEvent` | onLevelUnload |  | 
| `PlayerExposureChangeEvent` | onPlayerExposureChangeEvent |  | 
| `PossessEvent` | onPossess |  | 
| `ReloadJsonEvent` | onReloadJson |  | 
| `PossessEvent` | onUnpossess |  | 


## `EventMessage`

```csharp
public class ThunderRoad.EventMessage
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | duration |  | 
| `Int32` | priority |  | 
| `String` | text |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DebugLog(`String` text) |  | 
| `void` | DebugLogObject(`Object` obj) |  | 
| `void` | ShowMessage() |  | 
| `void` | ShowMessage(`String` text) |  | 
| `void` | StopMessage() |  | 


## `EventTime`

```csharp
public enum ThunderRoad.EventTime
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | OnStart |  | 
| `1` | OnEnd |  | 


## `ExcludeBelowPlaneColliderSamplingProvider`

```csharp
public class ThunderRoad.ExcludeBelowPlaneColliderSamplingProvider
    : SamplingProviderBase, IActiveSamplingProvider

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Collider>` | excludeBelowColliders |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | Name |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | InitializeSamplingProvider() |  | 
| `Boolean` | IsSamplingPositionActive(`Vector3` pos) |  | 


## `ExcludeInsideColliderSamplingProvider`

```csharp
public class ThunderRoad.ExcludeInsideColliderSamplingProvider
    : SamplingProviderBase, IActiveSamplingProvider

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | convexForced |  | 
| `Collider[]` | excludeColliders |  | 
| `Boolean[]` | excludeCollidersConvex |  | 
| `List<Transform>` | excludeRootColliders |  | 
| `Boolean` | forceConvex |  | 
| `Collider[]` | hitColliders |  | 
| `Int32` | hitCollidersCount |  | 
| `LayerMask` | layerMask |  | 
| `Single` | pointRadius |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | Name |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | InitializeSamplingProvider() |  | 
| `Boolean` | IsSamplingPositionActive(`Vector3` pos) |  | 
| `void` | RestoreConvex() |  | 


## `ExpressionData`

```csharp
public class ThunderRoad.ExpressionData
    : CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | browsIn |  | 
| `AnimationCurve` | curve |  | 
| `Single` | headLeft_Right |  | 
| `Single` | headTiltLeft_Right |  | 
| `Single` | headUp_Down |  | 
| `Single` | jawForward_Back |  | 
| `Single` | jawLeft_Right |  | 
| `Single` | jawOpen_Close |  | 
| `Single` | leftBrowUp_Down |  | 
| `Single` | leftCheekPuff_Squint |  | 
| `Single` | leftEyeIn_Out |  | 
| `Single` | leftEyeOpen_Close |  | 
| `Single` | leftEyeUp_Down |  | 
| `Single` | leftLowerLipUp_Down |  | 
| `Single` | leftMouthSmile_Frown |  | 
| `Single` | leftUpperLipUp_Down |  | 
| `Single` | midBrowUp_Down |  | 
| `Single` | mouthLeft_Right |  | 
| `Single` | mouthNarrow_Pucker |  | 
| `Single` | mouthUp_Down |  | 
| `Single` | neckLeft_Right |  | 
| `Single` | neckTiltLeft_Right |  | 
| `Single` | neckUp_Down |  | 
| `Single` | noseSneer |  | 
| `Single` | rightBrowUp_Down |  | 
| `Single` | rightCheekPuff_Squint |  | 
| `Single` | rightEyeIn_Out |  | 
| `Single` | rightEyeOpen_Close |  | 
| `Single` | rightEyeUp_Down |  | 
| `Single` | rightLowerLipUp_Down |  | 
| `Single` | rightMouthSmile_Frown |  | 
| `Single` | rightUpperLipUp_Down |  | 
| `Single` | tongueCurl |  | 
| `Single` | tongueLeft_Right |  | 
| `Single` | tongueOut |  | 
| `Single` | tongueUp_Down |  | 
| `Single` | tongueWide_Narrow |  | 


## `Extensions`

```csharp
public static class ThunderRoad.Extensions

```

Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | Clone(this `Collider` collider, `GameObject` gameObject) |  | 
| `SphereCollider` | Clone(this `SphereCollider` collider, `GameObject` gameObject) |  | 
| `CapsuleCollider` | Clone(this `CapsuleCollider` collider, `GameObject` gameObject) |  | 
| `BoxCollider` | Clone(this `BoxCollider` collider, `GameObject` gameObject) |  | 
| `MeshCollider` | Clone(this `MeshCollider` collider, `GameObject` gameObject) |  | 
| `T` | CloneJson(this `T` source) |  | 
| `String` | FormatBytes(this `Int64` bytes) |  | 
| `Single` | GetFirstTime(this `AnimationCurve` animationCurve) |  | 
| `Single` | GetFirstValue(this `AnimationCurve` animationCurve) |  | 
| `Single` | GetLastTime(this `AnimationCurve` animationCurve) |  | 
| `Single` | GetLastValue(this `AnimationCurve` animationCurve) |  | 
| `Boolean` | HasFlagNoGC(this `Type` flags, `Type` value) |  | 
| `Boolean` | HasFlagNoGC(this `PenetrationTempModifier` flags, `PenetrationTempModifier` value) |  | 
| `Boolean` | HasFlagNoGC(this `TierFilter` flags, `TierFilter` value) |  | 
| `Boolean` | HasFlagNoGC(this `TierFilter` flags, `TierFilter` value) |  | 
| `Boolean` | HasFlagNoGC(this `TypeFilter` flags, `TypeFilter` value) |  | 
| `Boolean` | HasFlagNoGC(this `DamageTypeFilter` flags, `DamageTypeFilter` value) |  | 
| `Boolean` | HasFlagNoGC(this `PenetrationFilter` flags, `PenetrationFilter` value) |  | 
| `Boolean` | HasFlagNoGC(this `DamagerFilter` flags, `DamagerFilter` value) |  | 
| `Boolean` | HasFlagNoGC(this `PlateformFilter` flags, `PlateformFilter` value) |  | 
| `Boolean` | HasFlagNoGC(this `ForceLiftCondition` flags, `ForceLiftCondition` value) |  | 
| `Boolean` | PointInRadius(this `Vector3` vectorA, `Vector3` vectorB, `Single` radius) |  | 
| `Boolean` | PointInRadius(this `Vector3` vectorA, `Vector3` vectorB, `Single` radius, `Single&` radiusDistanceRatio) |  | 
| `Vector3` | Round(this `Vector3` vector3, `Int32` decimalPlaces = 2) |  | 
| `void` | SetGlobalScale(this `Transform` transform, `Vector3` globalScale) |  | 
| `void` | SetTargetRotation(this `ConfigurableJoint` joint, `Quaternion` targetWorldRotation, `Quaternion` startWorldRotation) |  | 
| `void` | SetTargetRotationLocal(this `ConfigurableJoint` joint, `Quaternion` targetLocalRotation, `Quaternion` startLocalRotation) |  | 
| `List<T>` | Shuffle(this `List<T>` list) |  | 
| `T[]` | Shuffle(this `T[]` array) |  | 
| `Single` | SignedAngleFromDirection(this `Vector3` fromdir, `Vector3` todir, `Vector3` referenceup) |  | 
| `Vector3` | ToXZ(this `Vector3` fromdir) |  | 
| `Vector3` | ToYZ(this `Vector3` fromdir) |  | 


## `FaceCam`

```csharp
public class ThunderRoad.FaceCam
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | useWorldUp |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Update() |  | 


## `FeetClimber`

```csharp
public class ThunderRoad.FeetClimber
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Creature` | creature |  | 
| `Foot` | footLeft |  | 
| `Single` | footMaxAngle |  | 
| `Foot` | footRight |  | 
| `Single` | footSpeed |  | 
| `Boolean` | initialized |  | 
| `Single` | lastSweep |  | 
| `Single` | legLenghtMultiplier |  | 
| `Single` | legToHeadMaxAngle |  | 
| `Single` | minFootSpacing |  | 
| `Single` | moveOutWeight |  | 
| `Boolean` | showDebug |  | 
| `Int32` | sphereCastHitCount |  | 
| `RaycastHit[]` | sphereCastHits |  | 
| `Single` | sphereCastRadius |  | 
| `Single` | stepAngle |  | 
| `Single` | sweepAngle |  | 
| `Single` | sweepMaxHorizontalAngle |  | 
| `Single` | sweepMaxVerticalAngle |  | 
| `Single` | sweepMinDelay |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | CastSweep() |  | 
| `Foot` | GetFoot(`Side` side) |  | 
| `Single` | GetSweepDistance() |  | 
| `void` | Init() |  | 
| `void` | OnDrawGizmos() |  | 
| `Boolean` | SphereCastAngle(`Single` verticalAngle, `Single` horizontalAngle, `RaycastHit&` hitInfo) |  | 
| `void` | SphereCastVertical(`Single` horizontalAngle) |  | 
| `void` | Update() |  | 


## `FileManager`

```csharp
public class ThunderRoad.FileManager

```

Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | defaultFolderName |  | 
| `String` | modFolderName |  | 
| `Boolean` | useObb |  | 


Static Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | aaDefaultPath |  | 
| `String` | aaModPath |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | FileExist(`Type` type, `Source` source, `String` localPath) |  | 
| `String[]` | GetFilePaths(`Type` type, `Source` source, `String` localPath = , `String` searchPattern = *.*) |  | 
| `String[]` | GetFolderNames(`Type` type, `Source` source, `String` localPath = ) |  | 
| `String[]` | GetFullFilePaths(`Type` type, `Source` source, `String` localPath = , `String` searchPattern = *.*) |  | 
| `String` | GetFullPath(`Type` type, `Source` source, `String` relativePath = ) |  | 
| `List<ModData>` | GetOrderedMods() |  | 
| `String` | GetRelativePath(`String` relativeTo, `String` path) |  | 
| `String` | ReadAllText(`Type` type, `Source` source, `String` localPath) |  | 
| `ReadFile[]` | ReadFiles(`Type` type, `Source` source, `String` localPath = , `String` searchPattern = *.*) |  | 


## `FilterLogic`

```csharp
public enum ThunderRoad.FilterLogic
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | AnyExcept |  | 
| `1` | NoneExcept |  | 


## `Finger`

```csharp
public enum ThunderRoad.Finger
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | Thumb |  | 
| `1` | Index |  | 
| `2` | Middle |  | 
| `3` | Ring |  | 
| `4` | Little |  | 


## `FleePoint`

```csharp
public class ThunderRoad.FleePoint
    : MonoBehaviour

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnDisable() |  | 
| `void` | OnEnable() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<FleePoint>` | list |  | 


## `Footstep`

```csharp
public class ThunderRoad.Footstep
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioSource` | audioSource |  | 
| `Single` | lastTime |  | 
| `MaterialData` | materialData |  | 
| `String` | materialId |  | 
| `Single` | maxVelocity |  | 
| `Locomotion` | playerLocomotion |  | 
| `Boolean` | playerLocomotionGroundFall |  | 
| `Vector3` | playerLocomotionGroundFallVelocity |  | 
| `RagdollPart` | ragdollPart |  | 
| `SphereCollider` | sphereCollider |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | OnPlayerLocomotionGroundEvent(`Vector3` groundPoint, `Vector3` velocity, `Collider` groundCollider) |  | 


## `FxController`

```csharp
public class ThunderRoad.FxController
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | dampenedSpeed |  | 
| `Boolean` | initialized |  | 
| `Single` | intensity |  | 
| `List<FxModule>` | modules |  | 
| `Boolean` | playOnStart |  | 
| `Rigidbody` | rb |  | 
| `Single` | speed |  | 
| `Boolean` | velocityToSpeed |  | 
| `Single` | velocityToSpeedDampening |  | 
| `Vector2` | velocityToSpeedRange |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Play() |  | 
| `void` | Refresh() |  | 
| `void` | SetIntensity(`Single` intensity) |  | 
| `void` | SetSpeed(`Single` speed) |  | 
| `void` | Stop() |  | 
| `void` | Update() |  | 


## `FxModule`

```csharp
public class ThunderRoad.FxModule
    : MonoBehaviour

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | IsPlaying() |  | 
| `void` | Play() |  | 
| `void` | SetIntensity(`Single` intensity) |  | 
| `void` | SetSpeed(`Single` speed) |  | 
| `void` | Stop() |  | 


## `FxModuleAudio`

```csharp
public class ThunderRoad.FxModuleAudio
    : FxModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioMixerName` | audioMixer |  | 
| `Boolean` | doNoise |  | 
| `Boolean` | hasNoise |  | 
| `AnimationCurve` | highPassCutoffFrequencyCurve |  | 
| `AudioHighPassFilter` | highPassFilter |  | 
| `EffectLink` | highPassFilterEffectLink |  | 
| `AnimationCurve` | highPassResonanceQCurve |  | 
| `Boolean` | isPlaying |  | 
| `AudioContainer` | loopAudioContainer |  | 
| `String` | loopAudioContainerAddress |  | 
| `AudioSource` | loopAudioSource |  | 
| `Single` | loopVolumeDb |  | 
| `AnimationCurve` | lowPassCutoffFrequencyCurve |  | 
| `AudioLowPassFilter` | lowPassFilter |  | 
| `EffectLink` | lowPassFilterEffectLink |  | 
| `AnimationCurve` | lowPassResonanceQCurve |  | 
| `Noise` | noise |  | 
| `AudioSource` | oneShotAudioSource |  | 
| `AnimationCurve` | pitchCurve |  | 
| `EffectLink` | pitchEffectLink |  | 
| `AudioContainer` | playAudioContainer |  | 
| `String` | playAudioContainerAddress |  | 
| `Single` | playVolumeDb |  | 
| `AnimationCurve` | reverbDryLevelCurve |  | 
| `AudioReverbFilter` | reverbFilter |  | 
| `EffectLink` | reverbFilterEffectLink |  | 
| `AudioContainer` | stopAudioContainer |  | 
| `String` | stopAudioContainerAddress |  | 
| `Single` | stopVolumeDb |  | 
| `Boolean` | useHighPassFilter |  | 
| `Boolean` | useLowPassFilter |  | 
| `Boolean` | useReverbFilter |  | 
| `AnimationCurve` | volumeCurve |  | 
| `EffectLink` | volumeEffectLink |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Play() |  | 
| `void` | SetIntensity(`Single` intensity) |  | 
| `void` | SetSpeed(`Single` speed) |  | 
| `void` | SetVariation(`Single` value, `EffectLink` effectLink) |  | 
| `void` | Stop() |  | 
| `void` | TryCreateOneShootAudioSource() |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | DecibelToLinear(`Single` dB) |  | 
| `Single` | LinearToDecibel(`Single` linear) |  | 


## `FxModuleAudioLoop`

```csharp
public class ThunderRoad.FxModuleAudioLoop
    : FxModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | abnormalNoise |  | 
| `String` | audioClipAddress |  | 
| `AssetReference` | audioClipReference |  | 
| `AudioMixerName` | audioMixer |  | 
| `AudioSource` | audioSource |  | 
| `Boolean` | clipLoadedFromAddressable |  | 
| `Boolean` | hasNoise |  | 
| `AnimationCurve` | highPassCutoffFrequencyCurve |  | 
| `AudioHighPassFilter` | highPassFilter |  | 
| `Link` | highPassFilterLink |  | 
| `AnimationCurve` | highPassResonanceQCurve |  | 
| `AnimationCurve` | lowPassCutoffFrequencyCurve |  | 
| `AudioLowPassFilter` | lowPassFilter |  | 
| `Link` | lowPassFilterLink |  | 
| `AnimationCurve` | lowPassResonanceQCurve |  | 
| `Noise` | noise |  | 
| `AnimationCurve` | pitchCurve |  | 
| `Link` | pitchLink |  | 
| `Boolean` | playOnLoad |  | 
| `AnimationCurve` | reverbDryLevelCurve |  | 
| `AudioReverbFilter` | reverbFilter |  | 
| `Link` | reverbFilterLink |  | 
| `Single` | volume |  | 
| `AnimationCurve` | volumeCurve |  | 
| `Single` | volumeDb |  | 
| `Link` | volumeLink |  | 
| `Single` | volumeMultiplier |  | 
| `AnimationCurve` | volumeMultiplierCurve |  | 
| `Link` | volumeMultiplierLink |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | IsPlaying() |  | 
| `void` | Play() |  | 
| `void` | SetIntensity(`Single` intensity) |  | 
| `void` | SetSpeed(`Single` speed) |  | 
| `void` | SetVariation(`Single` value, `Link` link) |  | 
| `void` | Stop() |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | DecibelToLinear(`Single` dB) |  | 
| `Single` | LinearToDecibel(`Single` linear) |  | 


## `FxModuleAudioOnce`

```csharp
public class ThunderRoad.FxModuleAudioOnce
    : FxModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | abnormalNoise |  | 
| `String` | audioClipAddress |  | 
| `AssetReference` | audioClipReference |  | 
| `AudioMixerName` | audioMixer |  | 
| `AudioSource` | audioSource |  | 
| `Boolean` | clipLoadedFromAddressable |  | 
| `PlayEvent` | playEvent |  | 
| `Boolean` | playOnLoad |  | 
| `Single` | volumeDb |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | IsPlaying() |  | 
| `void` | Play() |  | 
| `void` | Stop() |  | 


## `FxModuleLight`

```csharp
public class ThunderRoad.FxModuleLight
    : FxModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | currentLightIntensity |  | 
| `Boolean` | flicker |  | 
| `Single` | flickerIntensityReduction |  | 
| `Single` | flickerMaxSpeed |  | 
| `Single` | flickerMinSpeed |  | 
| `Light` | light |  | 
| `Single` | orgLightIntensity |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Play() |  | 
| `void` | RefreshLightIntensity() |  | 
| `void` | SetIntensity(`Single` intensity) |  | 
| `void` | SetSpeed(`Single` speed) |  | 
| `void` | Stop() |  | 


## `FxModuleMaterial`

```csharp
public class ThunderRoad.FxModuleMaterial
    : FxModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Color>` | colorProperties |  | 
| `List<Float>` | floatProperties |  | 
| `List<Property>` | intensityProperties |  | 
| `Renderer` | meshRenderer |  | 
| `List<Property>` | speedProperties |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | SetIntensity(`Single` intensity) |  | 
| `void` | SetSpeed(`Single` speed) |  | 
| `void` | Stop() |  | 


## `FxModuleParticle`

```csharp
public class ThunderRoad.FxModuleParticle
    : FxModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AnimationCurve` | curveLifeTime |  | 
| `AnimationCurve` | emissionRateOverDistanceCurve |  | 
| `Link` | emissionRateOverDistanceLink |  | 
| `Vector2` | emissionRateOverDistanceRange |  | 
| `Single` | emissionRateOverDistanceReduction |  | 
| `AnimationCurve` | emissionRateOverTimeCurve |  | 
| `Link` | emissionRateOverTimeLink |  | 
| `Vector2` | emissionRateOverTimeRange |  | 
| `Single` | emissionRateOverTimeReduction |  | 
| `Link` | lifeTimeLink |  | 
| `Vector2` | lifeTimeRange |  | 
| `Single` | lifeTimeReduction |  | 
| `MinMaxCurve` | minMaxCurve |  | 
| `ParticleSystem` | particleSystem |  | 
| `MainModule` | particleSystemMain |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | IsPlaying() |  | 
| `void` | Play() |  | 
| `void` | SetEmissionRateOverDistance(`Single` value) |  | 
| `void` | SetEmissionRateOverTime(`Single` value) |  | 
| `void` | SetIntensity(`Single` intensity) |  | 
| `void` | SetLifetime(`Single` value) |  | 
| `void` | SetSpeed(`Single` speed) |  | 
| `void` | Stop() |  | 


## `FxModuleVfx`

```csharp
public class ThunderRoad.FxModuleVfx
    : FxModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Color>` | colorProperties |  | 
| `List<Float>` | floatProperties |  | 
| `List<Property>` | intensityProperties |  | 
| `List<Property>` | speedProperties |  | 
| `VisualEffect` | vfx |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | IsPlaying() |  | 
| `void` | Play() |  | 
| `void` | SetIntensity(`Single` intensity) |  | 
| `void` | SetSpeed(`Single` speed) |  | 
| `void` | Stop() |  | 


## `GameData`

```csharp
public class ThunderRoad.GameData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `PlateformParameters` | android |  | 
| `Boolean` | arcadeControlPanel |  | 
| `List<Category>` | categories |  | 
| `Int32` | cleanDeadLastInteractionDelay |  | 
| `Int32` | cleanObjectsLastInteractionDelay |  | 
| `CollisionDetection` | collisionDetection |  | 
| `Vector2` | collisionEnterVelocityRange |  | 
| `Vector2` | collisionStayVelocityRange |  | 
| `EffectData` | deathEffectData |  | 
| `String` | deathEffectId |  | 
| `Single` | deathSlowMoDuration |  | 
| `AnimationCurve` | deathSlowMoEnterCurve |  | 
| `AnimationCurve` | deathSlowMoExitCurve |  | 
| `Single` | deathSlowMoRatio |  | 
| `Boolean` | debugAdvanced |  | 
| `Boolean` | debugDungeonCaptureMemoryUsage |  | 
| `Boolean` | debugDungeonWaitPress |  | 
| `String` | defaultPlayerFemaleCreatureID |  | 
| `String` | defaultPlayerMaleCreatureID |  | 
| `EffectData` | defaultWheelOrbEffectData |  | 
| `String` | defaultWheelOrbEffectId |  | 
| `Boolean` | disableCharacterCustomization |  | 
| `Boolean` | disableCharacterDeletion |  | 
| `AudioContainer` | errorAudioGroup |  | 
| `String` | errorAudioGroupAddress |  | 
| `Experience` | experience |  | 
| `List<Faction>` | factions |  | 
| `Single` | fingerSpeed |  | 
| `Boolean` | fullscreen |  | 
| `List<GameMode>` | gameModes |  | 
| `String` | gameVersion |  | 
| `Haptics` | haptics |  | 
| `List<String>` | holderSlots |  | 
| `Honor` | honor |  | 
| `Int32` | itemIconResolution |  | 
| `EffectData` | itemWheelEffectData |  | 
| `String` | itemWheelEffectId |  | 
| `String` | levelStart |  | 
| `String` | levelStartModeName |  | 
| `Dictionary<String, Double>` | levelStartOptions |  | 
| `Boolean` | loadMods |  | 
| `GroundDetection` | locomotionGroundDetection |  | 
| `Int32` | maxCollisionStayCheckPerFrame |  | 
| `Int32` | maxObjectCollision |  | 
| `String` | menuPrefabAddress |  | 
| `String` | minModVersion |  | 
| `Single` | motionBlurIntensity |  | 
| `Boolean` | overrideSaveCharacters |  | 
| `Boolean` | overrideSaveOptions |  | 
| `PlateformParameters` | pc |  | 
| `Vector2` | penetrationVelocityEffectRange |  | 
| `PlateformParameters` | platformParameters |  | 
| `String` | playerHighlighterAddress |  | 
| `String` | savesFolder |  | 
| `Score` | score |  | 
| `Int32` | screenHeight |  | 
| `ScreenshotFormat` | screenshotFormat |  | 
| `Int32` | screenshotJpegQuality |  | 
| `Int32` | screenWidth |  | 
| `Boolean` | showControlPanelOnStart |  | 
| `List<SkillCluster>` | skillTree |  | 
| `HandPoseData` | SpellWheelCloseHandPoseData |  | 
| `String` | SpellWheelCloseHandPoseId |  | 
| `EffectData` | spellWheelEffectData |  | 
| `String` | spellWheelEffectId |  | 
| `HandPoseData` | SpellWheelOpenHandPoseData |  | 
| `String` | SpellWheelOpenHandPoseId |  | 
| `Single` | throwMultiplier |  | 
| `Single` | throwVelocity |  | 
| `HandPoseData` | uiPointingCloseHandPoseData |  | 
| `String` | uiPointingCloseHandPoseId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<ValueDropdownItem<String>>` | GetAllEffectID() |  | 
| `List<ValueDropdownItem<String>>` | GetAllHandPoseID() |  | 
| `List<ValueDropdownItem<String>>` | GetAllLevelID() |  | 
| `List<ValueDropdownItem<String>>` | GetCategories() |  | 
| `Category` | GetCategory(`String` name) |  | 
| `Category` | GetCategoryUnknown() |  | 
| `Category` | GetDamageCategory(`DamageType` damageType) |  | 
| `Faction` | GetFaction(`Int32` factionId) |  | 
| `List<ValueDropdownItem<Int32>>` | GetFactions() |  | 
| `GameMode` | GetGameMode(`String` gameModeId) |  | 
| `void` | OnCatalogRefresh() |  | 
| `IEnumerator` | OnCatalogRefreshCoroutine() |  | 
| `Boolean` | ShouldSerializearcadeControlPanel() |  | 


## `GameManager`

```csharp
public class ThunderRoad.GameManager
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioMixer` | audioMixer |  | 
| `List<String>` | buildLoadDefaultFolders |  | 
| `CollisionDebug` | collisionDebug |  | 
| `String[]` | commandLineArgs |  | 
| `PlatformStore` | currentPlatformStore |  | 
| `Boolean` | debugLoading |  | 
| `Int32` | defaultCharacterIndex |  | 
| `List<String>` | editorLoadDefaultFolders |  | 
| `LayerMask` | groundLayer |  | 
| `Boolean` | loadDll |  | 
| `Single` | meshRaycastBackDistance |  | 
| `Boolean` | meshRaycastDebug |  | 
| `Boolean` | meshRaycastDebugFailPause |  | 
| `Boolean` | meshRaycastDebugHitFleshPause |  | 
| `Single` | meshRaycastNormalToVelocityRatio |  | 
| `String` | minModVersion |  | 
| `Material` | mirrorMaterial |  | 
| `ObjectViewer` | objectViewer |  | 
| `Boolean` | pauseOnVRPresence |  | 
| `PlatformStoreEnum` | platformStore |  | 
| `Boolean` | platformStoreLoaded |  | 
| `String` | playerPrefabAddress |  | 
| `String` | spectatorAddress |  | 
| `Boolean` | useCommandLine |  | 
| `Int32` | versionBuild |  | 
| `Int32` | versionMajor |  | 
| `Int32` | versionMinor |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `List<ValueDropdownItem<String>>` | GetAllLevelID() |  | 
| `String` | GetVersionString(`Boolean` stripBuild = False) |  | 
| `IEnumerator` | Init() |  | 
| `void` | OnQuit() |  | 
| `void` | OnVRPresence(`Boolean` active) |  | 
| `void` | Pause(`Boolean` active) |  | 
| `void` | QuitGame() |  | 
| `void` | Update() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameManager` | _local |  | 
| `AudioMixerGroup[]` | audioMixerGroups |  | 
| `AudioMixerSnapshot` | audioMixerSnapshotDefault |  | 
| `AudioMixerSnapshot` | audioMixerSnapshotSlowmo |  | 
| `Boolean` | forceCalibration |  | 
| `Single` | forcePlayerHeight |  | 
| `Boolean` | initialized |  | 
| `Boolean` | isQuitting |  | 
| `String` | language |  | 
| `Int32[]` | layers |  | 
| `LIV` | liv |  | 
| `List<SceneInstance>` | loadedScenes |  | 
| `MenuBook` | menuPrefab |  | 
| `Options` | options |  | 
| `Single` | orgFixedTimeStep |  | 
| `Player` | playerPrefab |  | 
| `Transform` | poolTransform |  | 
| `SlowMotionState` | slowMotionState |  | 
| `EffectInstance` | slowTimeEffectInstance |  | 
| `Boolean` | timeStopped |  | 


Static Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameManager` | local |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AllowBloodEffects(`Boolean` active) |  | 
| `IEnumerator` | DebugWaitButtonPress() |  | 
| `AudioMixerGroup` | GetAudioMixerGroup(`AudioMixerName` audioMixerName) |  | 
| `String` | GetCurrentLevel() |  | 
| `Int32` | GetLayer(`LayerName` layerName) |  | 
| `Single` | GetTimeStepMultiplier() |  | 
| `void` | LoadLevel(`String` levelId, `String` modeName = null, `Dictionary<String, Double>` options = null) |  | 
| `void` | LoadLevel(`LevelData` levelData, `Mode` mode, `Dictionary<String, Double>` options = null) |  | 
| `void` | LoadOptions() |  | 
| `void` | ReloadJsonAndAssets() |  | 
| `IEnumerator` | ReloadJsonAndAssetsCoroutine() |  | 
| `void` | ReloadLevel(`Boolean` useSameSeed = False) |  | 
| `void` | SaveOptions(`Boolean` clear = False) |  | 
| `void` | Screenshot(`Camera` cam) |  | 
| `IEnumerator` | ScreenshotCoroutine() |  | 
| `void` | SetInfiniteArrows(`Boolean` active) |  | 
| `void` | SetInfiniteFocus(`Boolean` active) |  | 
| `void` | SetInfiniteImbue(`Boolean` active) |  | 
| `void` | SetInfiniteMana(`Boolean` active) |  | 
| `void` | SetLiv(`Boolean` active, `Player` player) |  | 
| `void` | SetPlayerFallDamage(`Boolean` active) |  | 
| `void` | SetPlayerInvincibility(`Boolean` active) |  | 
| `void` | SetSlowMotion(`Boolean` active, `Single` scale, `AnimationCurve` curve, `EffectData` effectData = null, `Boolean` snapshotTransition = True) |  | 
| `void` | SetTime(`Boolean` active) |  | 
| `void` | SetTimeScale(`Single` scale) |  | 
| `void` | StopSlowMotion() |  | 
| `String` | TryGetTranslation(`String` text, `String` value1 = null, `String` value2 = null) |  | 
| `void` | UnLoadLevel() |  | 


## `GameMode`

```csharp
public class ThunderRoad.GameMode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | allowLevelSelection |  | 
| `Boolean` | allowMenuOptions |  | 
| `Boolean` | allowMenuSandbox |  | 
| `Boolean` | defaultInfiniteArrows |  | 
| `Boolean` | defaultInfiniteImbue |  | 
| `Boolean` | defaultPlayerFallDamage |  | 
| `String` | defaultPlayerHomeContainerID |  | 
| `Boolean` | defaultPlayerInfiniteFocus |  | 
| `Boolean` | defaultPlayerInfiniteMana |  | 
| `Boolean` | defaultPlayerInvincibility |  | 
| `String` | description |  | 
| `String` | iconAddress |  | 
| `Texture2D` | iconLoaded |  | 
| `IResourceLocation` | iconLocation |  | 
| `String` | id |  | 
| `String` | levelCharacterSelection |  | 
| `String` | levelCharacterSelectionModeName |  | 
| `String` | levelHome |  | 
| `String` | levelHomeModeName |  | 
| `String` | name |  | 
| `Boolean` | resetApparels |  | 
| `Boolean` | resetSpells |  | 
| `State` | state |  | 
| `Boolean` | tutorialEnabled |  | 
| `String` | warning |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CheckPlayerSaveData(`PlayerCharacterData` playerCharacterData) |  | 
| `List<ValueDropdownItem<String>>` | GetAllLevelID() |  | 
| `void` | LoadPlayerSaveData(`PlayerCharacterData` playerCharacterData) |  | 
| `PlayerCharacterData` | NewPlayerSaveData() |  | 


## `Handle`

```csharp
public class ThunderRoad.Handle
    : Interactable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Rigidbody` | customRigidBody |  | 
| `HandleData` | data |  | 
| `Single` | defaultGrabAxisRatio |  | 
| `Boolean` | forceAutoDropWhenGrounded |  | 
| `Boolean` | forcePlayerJoint |  | 
| `List<RagdollHand>` | handlers |  | 
| `Int32` | handlersCount |  | 
| `List<Collider>` | handOverlapColliders |  | 
| `Vector3` | ikAnchorOffset |  | 
| `Item` | item |  | 
| `Boolean` | justGrabbed |  | 
| `Vector2` | lastPositionMultiplier |  | 
| `Vector2` | lastRotationMultiplier |  | 
| `Handle` | moveToHandle |  | 
| `Single` | moveToHandleAxisPos |  | 
| `HandleOrientation` | orientationDefaultLeft |  | 
| `HandleOrientation` | orientationDefaultRight |  | 
| `List<HandleOrientation>` | orientations |  | 
| `Rigidbody` | rb |  | 
| `Single` | reach |  | 
| `Handle` | releaseHandle |  | 
| `Single` | slideForce |  | 
| `Handle` | slideToBottomHandle |  | 
| `Single` | slideToHandleOffset |  | 
| `Handle` | slideToUpHandle |  | 
| `SpellCaster` | telekinesisHandler |  | 
| `Boolean` | usePlayerJoint |  | 


Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `GrabEvent` | Grabbed |  | 
| `GrabEvent` | UnGrabbed |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `HandleOrientation` | AddOrientation(`Side` side, `Vector3` position, `Quaternion` rotation) |  | 
| `void` | Attach(`RagdollHand` ragdollHand, `Boolean` usePhysic) |  | 
| `void` | Awake() |  | 
| `void` | CalculateReach() |  | 
| `InteractionResult` | CheckInteraction(`RagdollHand` ragdollHand) |  | 
| `void` | CheckOrientations() |  | 
| `GripInfo` | CreateGripPoint(`RagdollHand` ragdollHand, `Single` axisPosition, `HandleOrientation` orientation) |  | 
| `void` | FixedUpdate() |  | 
| `void` | ForcePlayerGrab() |  | 
| `Single` | GetDefaultAxisLocalPosition() |  | 
| `Vector3` | GetDefaultAxisPosition(`Side` side) |  | 
| `HandleOrientation` | GetDefaultOrientation(`Side` side) |  | 
| `Single` | GetNearestAxisPosition(`Vector3` position) |  | 
| `HandleOrientation` | GetNearestOrientation(`Transform` grip, `Side` side) |  | 
| `Vector3` | GetNearestPositionAlongAxis(`Vector3` position) |  | 
| `void` | HeldAction(`RagdollHand` ragdollHand, `Action` action) |  | 
| `Boolean` | HeldActionAvailable(`RagdollHand` ragdollHand, `Action` action) |  | 
| `Boolean` | HoldGripToGrab() |  | 
| `Boolean` | IsAllowed(`Side` side) |  | 
| `Boolean` | IsHanded() |  | 
| `void` | Load(`InteractableData` interactableData) |  | 
| `void` | OnDrawGizmosSelected() |  | 
| `void` | OnGrab(`RagdollHand` ragdollHand, `Single` axisPosition, `HandleOrientation` orientation, `Boolean` teleportToHand = False) |  | 
| `void` | OnPlayerLocomotionFlyEvent() |  | 
| `void` | OnPlayerLocomotionGroundEvent(`Vector3` groundPoint, `Vector3` velocity, `Collider` groundCollider) |  | 
| `void` | OnTelekinesisGrab(`SpellTelekinesis` spellTelekinesis) |  | 
| `void` | OnTelekinesisRelease(`SpellTelekinesis` spellTelekinesis, `Boolean` tryThrow, `Boolean&` throwing) |  | 
| `void` | OnTouchEnd(`RagdollHand` ragdollHand) |  | 
| `void` | OnTouchStart(`RagdollHand` ragdollHand) |  | 
| `void` | OnTouchStay(`RagdollHand` ragdollHand) |  | 
| `void` | OnUnGrab(`RagdollHand` ragdollHand, `Boolean` throwing) |  | 
| `void` | RefreshAllJointDrives() |  | 
| `void` | RefreshJointDrive() |  | 
| `void` | Release() |  | 
| `void` | SetJointConfig(`RagdollHand` handler, `Vector2` positionMultiplier, `Vector2` rotationMultiplier, `RotationDrive` rotationDrive) |  | 
| `void` | SetJointConfig(`ConfigurableJoint` joint, `RagdollHand` handler, `Vector2` positionMultiplier, `Vector2` rotationMultiplier, `Single` maxPositionForce, `Single` maxRotationForce, `RotationDrive` rotationDrive, `Single` limit = 0) |  | 
| `void` | SetJointDrive(`Vector2` positionMultiplier, `Vector2` rotationMultiplier) |  | 
| `void` | SetJointToTwoHanded(`Side` dominantSide, `Single` rotationMultiplier = 1) |  | 
| `void` | SetSliding(`RagdollHand` ragdollHand, `Boolean` active) |  | 
| `void` | SetTelekinesis(`Boolean` active) |  | 
| `Boolean` | TryTouchAction(`RagdollHand` ragdollHand, `Action` action) |  | 
| `void` | Update() |  | 
| `void` | UpdateAutoRotate() |  | 
| `void` | UpdateSliding() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Side` | dominantHand |  | 
| `Boolean` | globalForceXYZ |  | 
| `Single` | globalPositionDamperMultiplier |  | 
| `Single` | globalPositionSpringMultiplier |  | 
| `Single` | globalRotationDamperMultiplier |  | 
| `Single` | globalRotationSpringMultiplier |  | 
| `Boolean` | holdGrip |  | 
| `TwoHandedMode` | twoHandedMode |  | 


## `HandleData`

```csharp
public class ThunderRoad.HandleData
    : InteractableData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | allowSlidingWithBothHand |  | 
| `Boolean` | allowSpellFire |  | 
| `Boolean` | allowSpellMenu |  | 
| `Boolean` | allowSteal |  | 
| `Boolean` | allowSwap |  | 
| `Boolean` | allowTelekinesis |  | 
| `Boolean` | disabledOnSnap |  | 
| `Boolean` | disableHandCollider |  | 
| `Boolean` | disablePinchGrab |  | 
| `Boolean` | dominantWhenTwoHanded |  | 
| `Boolean` | forceAllowTwoHanded |  | 
| `Boolean` | forceClimbing |  | 
| `Boolean` | forceHoldGripToGrab |  | 
| `Boolean` | forcePlayerPhysicLink |  | 
| `EffectData` | grabEffectData |  | 
| `String` | grabEffectId |  | 
| `Single` | handlerLocomotionSpeedMultiplier |  | 
| `HandPoseData` | handPoseData |  | 
| `String` | handPoseId |  | 
| `Boolean` | ignoreSnap |  | 
| `Single` | positionDamperMultiplier |  | 
| `Single` | positionSpringMultiplier |  | 
| `Boolean` | rotateAroundAxis |  | 
| `Single` | rotationDamper2hMultiplier |  | 
| `Single` | rotationDamperMultiplier |  | 
| `RotationDrive` | rotationDrive |  | 
| `Single` | rotationSpring2hMultiplier |  | 
| `Single` | rotationSpringMultiplier |  | 
| `Boolean` | setCenterOfMassTohandle |  | 
| `Single` | slideFxMaxVelocity |  | 
| `Single` | slideFxMinVelocity |  | 
| `Single` | slideMaxDamper |  | 
| `Single` | slideMinDamper |  | 
| `Single` | slideMotorAcceleration |  | 
| `SlideMotorDirection` | slideMotorDir |  | 
| `Single` | slideMotorMaxForce |  | 
| `HandPoseData` | spellFireHandPoseData |  | 
| `String` | spellFireHandPoseId |  | 
| `Vector3` | spellFireMagicOffset |  | 
| `Single` | telekinesisMaxDistanceMultiplier |  | 
| `Single` | telekinesisPositionDamperMultiplier |  | 
| `Single` | telekinesisPositionMaxForceMultiplier |  | 
| `Single` | telekinesisPositionSpringMultiplier |  | 
| `Single` | telekinesisPullRepelMultiplier |  | 
| `Single` | telekinesisRotationDamperMultiplier |  | 
| `Single` | telekinesisRotationMaxForceMultiplier |  | 
| `Single` | telekinesisRotationSpringMultiplier |  | 
| `Boolean` | useDefaultGripForHolder |  | 
| `Boolean` | useWYZWhenTwoHanded |  | 
| `Boolean` | warnIfNotAllowed |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<ValueDropdownItem<String>>` | GetAllEffectID() |  | 
| `List<ValueDropdownItem<String>>` | GetAllHandPoseID() |  | 
| `void` | OnCatalogRefresh() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Side` | dominantHand |  | 
| `String` | tagTkDefault |  | 
| `String` | tagTkDefaultLeft |  | 
| `String` | tagTkDefaultRight |  | 
| `String` | tagTkRagdoll |  | 
| `String` | tagTkRagdollLeft |  | 
| `String` | tagTkRagdollRight |  | 
| `TwoHandedMode` | twoHandedMode |  | 


## `HandleOrientation`

```csharp
public class ThunderRoad.HandleOrientation
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Handle` | handle |  | 
| `Mesh` | handMesh |  | 
| `Side` | side |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnDrawGizmosSelected() |  | 
| `void` | OnValidate() |  | 
| `void` | UpdateName() |  | 


## `HandleRagdoll`

```csharp
public class ThunderRoad.HandleRagdoll
    : Handle

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Transform` | bodyAnchor |  | 
| `HandleRagdollData` | handleRagdollData |  | 
| `Boolean` | isBackGrab |  | 
| `RagdollPart` | ragdollPart |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `Boolean` | HoldGripToGrab() |  | 
| `void` | Load(`InteractableData` interactableData) |  | 
| `void` | OnGrab(`RagdollHand` ragdollHand, `Single` axisPosition, `HandleOrientation` orientation, `Boolean` teleportToHand = False) |  | 
| `void` | OnTelekinesisGrab(`SpellTelekinesis` spellTelekinesis) |  | 
| `void` | OnTelekinesisRelease(`SpellTelekinesis` spellTelekinesis, `Boolean` tryThrow, `Boolean&` throwing) |  | 
| `void` | OnUnGrab(`RagdollHand` ragdollHand, `Boolean` throwing) |  | 
| `void` | RefreshJointAndCollision() |  | 
| `void` | ResetStep() |  | 
| `void` | Update() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | grabThrowLevel |  | 
| `Boolean` | holdGripRagdoll |  | 


## `HandleRagdollData`

```csharp
public class ThunderRoad.HandleRagdollData
    : HandleData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Type>` | activateCollisionOnParts |  | 
| `Boolean` | allowRotationIK |  | 
| `Behaviour` | behaviour |  | 
| `BodyTurnDirection` | bodyTurnDirection |  | 
| `Cardinal` | cardinal |  | 
| `Boolean` | changeHeight |  | 
| `ForceLiftCondition` | forceLiftGrabCondition |  | 
| `ForceLiftCondition` | forceLiftTKCondition |  | 
| `Single` | highTwistLimit |  | 
| `Single` | IkPositionWeight |  | 
| `Single` | IkRotationWeight |  | 
| `Boolean` | invertLowHighOnBack |  | 
| `LiftBehaviour` | liftBehaviour |  | 
| `Single` | liftOffset |  | 
| `Part` | liftPartReference |  | 
| `Single` | lowTwistLimit |  | 
| `Boolean` | moveStep |  | 
| `List<Type>` | overrideCharJointLimitsOnParts |  | 
| `Single` | releaseArmDamper |  | 
| `Single` | releaseArmSpring |  | 
| `Part` | stepPartReference |  | 
| `Single` | stepSpeedMultiplier |  | 
| `Single` | stepThresholdMultiplier |  | 
| `Single` | swing1Limit |  | 
| `Boolean` | useIK |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CheckForceLiftCondition(`Creature` creature) |  | 
| `List<ValueDropdownItem<String>>` | GetAllDamagerID() |  | 


## `HandPose`

```csharp
public class ThunderRoad.HandPose
    : ScriptableObject

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Fingers` | left |  | 
| `Fingers` | right |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Fingers` | GetFingers(`Side` side) |  | 
| `void` | Save(`Side` side) |  | 
| `void` | SaveFinger(`Finger` finger1, `Finger` finger2) |  | 


## `HandPoseData`

```csharp
public class ThunderRoad.HandPoseData
    : CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | allowIndexTracking |  | 
| `Boolean` | allowLittleTracking |  | 
| `Boolean` | allowMiddleTracking |  | 
| `Boolean` | allowRingTracking |  | 
| `Boolean` | allowThumbTracking |  | 
| `Boolean` | indexNoTrigger |  | 
| `List<Pose>` | poses |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | GetCurrentVersion() |  | 
| `HandPose` | GetHandPose(`Creature` creature) |  | 
| `IEnumerator` | OnCatalogRefreshCoroutine() |  | 


## `Highlighter`

```csharp
public class ThunderRoad.Highlighter
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | active |  | 
| `Transform` | anchor |  | 
| `Single` | autoMinSize |  | 
| `Single` | autoSizeDistanceRatio |  | 
| `Single` | axisPosition |  | 
| `Canvas` | canvas |  | 
| `Single` | currentRotation |  | 
| `Color` | defaultColor |  | 
| `Text` | designationText |  | 
| `Boolean` | faceCamUseWorldUp |  | 
| `RawImage` | outlineDefault |  | 
| `Image` | outlineLineBottom |  | 
| `Text` | outlineLineBottomText |  | 
| `Image` | outlineLineUp |  | 
| `Text` | outlineLineUpText |  | 
| `RawImage` | outlineTK |  | 
| `Boolean` | rotate |  | 
| `Single` | rotateSpeed |  | 
| `Side` | side |  | 
| `Text` | titleText |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | Hide() |  | 
| `void` | SetOutlineColor(`Color` color) |  | 
| `void` | SetTextColor(`Color` color) |  | 
| `void` | Show(`Transform` anchor, `String` title, `String` designation, `Style` style = Default, `Single` autoMinSize = 1, `Boolean` rotate = False) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | isEnabled |  | 
| `Highlighter` | left |  | 
| `Highlighter` | right |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Highlighter` | GetSide(`Side` side) |  | 


## `HingeEffect`

```csharp
public class ThunderRoad.HingeEffect
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | currentIntensity |  | 
| `String` | effectId |  | 
| `EffectInstance` | effectInstance |  | 
| `HingeJoint` | joint |  | 
| `Rigidbody` | jointRb |  | 
| `Boolean` | loaded |  | 
| `Single` | maxTorque |  | 
| `Single` | minTorque |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<ValueDropdownItem<String>>` | GetAllEffectID() |  | 
| `void` | Load(`String` effectId, `Single` minTorque, `Single` maxTorque) |  | 
| `void` | Update() |  | 


## `Holder`

```csharp
public class ThunderRoad.Holder
    : Interactable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioContainer` | audioContainer |  | 
| `Coroutine` | cleanItemsCoroutine |  | 
| `Creature` | creature |  | 
| `Int32` | currentQuantity |  | 
| `DrawSlot` | drawSlot |  | 
| `String` | editorTargetAnchor |  | 
| `List<Content>` | extraContents |  | 
| `Boolean` | grabChildHolder |  | 
| `List<Collider>` | ignoredColliders |  | 
| `List<Item>` | items |  | 
| `Holder` | parentHolder |  | 
| `Item` | parentItem |  | 
| `List<Transform>` | slots |  | 
| `List<Item>` | startObjects |  | 
| `Boolean` | useAnchor |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `HolderData` | data |  | 


Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `HolderDelegate` | Snapped |  | 
| `HolderDelegate` | UnSnapped |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AlignObject(`Item` item) |  | 
| `void` | Awake() |  | 
| `Boolean` | CanTouch(`RagdollHand` ragdollHand) |  | 
| `InteractionResult` | CheckInteraction(`RagdollHand` ragdollHand) |  | 
| `String` | GetQuantityText() |  | 
| `Holder` | GetRootHolder() |  | 
| `Boolean` | GrabFromHandle() |  | 
| `Boolean` | HasSlotFree() |  | 
| `void` | Load(`InteractableData` interactableData) |  | 
| `Boolean` | ObjectAllowed(`Item` item) |  | 
| `void` | OnDrawGizmosSelected() |  | 
| `void` | OnTouchEnd(`RagdollHand` ragdollHand) |  | 
| `void` | OnTouchStart(`RagdollHand` ragdollHand) |  | 
| `void` | OnValidate() |  | 
| `void` | RefreshChildAndParentHolder() |  | 
| `void` | ShowHint(`RagdollHand` ragdollHand) |  | 
| `Boolean` | SlotAllowed(`String` slot) |  | 
| `void` | Snap(`Item` item, `Boolean` silent = False) |  | 
| `void` | Start() |  | 
| `Boolean` | TryTouchAction(`RagdollHand` ragdollHand, `Action` action) |  | 
| `void` | UnSnap(`Item` item, `Boolean` silent = False) |  | 
| `void` | UnSnapAll() |  | 
| `Item` | UnSnapOne() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | showHudHighlighter |  | 


## `HolderData`

```csharp
public class ThunderRoad.HolderData
    : InteractableData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | allowTeleGrab |  | 
| `String` | audioContainerAddress |  | 
| `IResourceLocation` | audioContainerLocation |  | 
| `Single` | cleanItemsDuration |  | 
| `Single` | cleanItemsStep |  | 
| `Boolean` | delegateToParentHolder |  | 
| `Boolean` | disableObjectProximityHighlighter |  | 
| `Boolean` | forceAllowTouchOnPlayer |  | 
| `Boolean` | grabFromHandle |  | 
| `GrabTeleport` | grabTeleport |  | 
| `Boolean` | hideFromFpv |  | 
| `Boolean` | highlighterPlayerView |  | 
| `Boolean` | locked |  | 
| `Int32` | maxQuantity |  | 
| `Boolean` | playerGrabFromHandle |  | 
| `List<String>` | slots |  | 
| `String` | spawnItemID |  | 
| `Int32` | spawnQuantity |  | 
| `FilterLogic` | tagFilter |  | 
| `String` | targetAnchor |  | 
| `Boolean` | warnIfInUse |  | 
| `Boolean` | warnIfLocked |  | 
| `Boolean` | warnIfNotAllowed |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<ValueDropdownItem<String>>` | GetAllHolderSlots() |  | 
| `List<ValueDropdownItem<String>>` | GetAllItemID() |  | 
| `IEnumerator` | OnCatalogRefreshCoroutine() |  | 


## `HueColorName`

```csharp
public enum ThunderRoad.HueColorName
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | Lime |  | 
| `1` | Green |  | 
| `2` | Aqua |  | 
| `3` | Blue |  | 
| `4` | Navy |  | 
| `5` | Purple |  | 
| `6` | Pink |  | 
| `7` | Red |  | 
| `8` | Orange |  | 
| `9` | Yellow |  | 
| `10` | White |  | 


## `IconManager`

```csharp
public class ThunderRoad.IconManager

```

Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | SetIcon(`GameObject` gObj, `LabelIcon` icon) |  | 
| `void` | SetIcon(`GameObject` gObj, `Icon` icon) |  | 
| `void` | SetIcon(`GameObject` gObj, `Texture2D` texture) |  | 


## `IkController`

```csharp
public class ThunderRoad.IkController
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Creature` | creature |  | 
| `Transform` | eyesTarget |  | 
| `Transform` | fingerLeftIndexTarget |  | 
| `Transform` | fingerLeftLittleTarget |  | 
| `Transform` | fingerLeftMiddleTarget |  | 
| `Transform` | fingerLeftRingTarget |  | 
| `Transform` | fingerLeftThumbTarget |  | 
| `Transform` | fingerRightIndexTarget |  | 
| `Transform` | fingerRightLittleTarget |  | 
| `Transform` | fingerRightMiddleTarget |  | 
| `Transform` | fingerRightRingTarget |  | 
| `Transform` | fingerRightThumbTarget |  | 
| `Boolean` | footLeftEnabled |  | 
| `Transform` | footLeftTarget |  | 
| `Boolean` | footRightEnabled |  | 
| `Transform` | footRightTarget |  | 
| `Boolean` | fullbody |  | 
| `Boolean` | handLeftEnabled |  | 
| `Transform` | handLeftTarget |  | 
| `Boolean` | handRightEnabled |  | 
| `Transform` | handRightTarget |  | 
| `Boolean` | headEnabled |  | 
| `Transform` | headTarget |  | 
| `Boolean` | hipsEnabled |  | 
| `Transform` | hipsTarget |  | 
| `Boolean` | shoulderLeftEnabled |  | 
| `Transform` | shoulderLeftTarget |  | 
| `Boolean` | shoulderRightEnabled |  | 
| `Transform` | shoulderRightTarget |  | 
| `Boolean` | turnBodyByHeadAndHands |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | initialized |  | 


Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `LateUpdateDelegate` | OnPostIKUpdateEvent |  | 
| `LateUpdateDelegate` | OnPreIKUpdateEvent |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddLocomotionDeltaPosition(`Vector3` delta) |  | 
| `void` | AddLocomotionDeltaRotation(`Quaternion` delta, `Vector3` pivot) |  | 
| `void` | Awake() |  | 
| `FootBoneTarget` | GetFootBoneTarget() |  | 
| `Single` | GetHandPositionWeight(`Side` side) |  | 
| `Single` | GetHandRotationWeight(`Side` side) |  | 
| `Single` | GetHeadWeight() |  | 
| `Single` | GetHipsWeight() |  | 
| `Single` | GetLocomotionWeight() |  | 
| `Single` | GetLookAtWeight() |  | 
| `void` | PostIKUpdate() |  | 
| `void` | PreIKUpdate() |  | 
| `void` | SetFootAnchor(`Side` side, `Transform` anchor) |  | 
| `void` | SetFootAnchor(`Side` side, `Transform` anchor, `Quaternion` toesRotation) |  | 
| `void` | SetFootPull(`Side` side, `Single` value) |  | 
| `void` | SetFootState(`Side` side, `Boolean` active) |  | 
| `void` | SetFootWeight(`Side` side, `Single` positionWeight, `Single` rotationWeight) |  | 
| `void` | SetFullbody(`Boolean` active) |  | 
| `void` | SetHandAnchor(`Side` side, `Transform` anchor) |  | 
| `void` | SetHandAnchor(`Side` side, `Transform` anchor, `Quaternion` palmRotation) |  | 
| `void` | SetHandState(`Side` side, `Boolean` positionEnabled, `Boolean` rotationEnabled) |  | 
| `void` | SetHandWeight(`Side` side, `Single` positionWeight, `Single` rotationWeight) |  | 
| `void` | SetHeadAnchor(`Transform` anchor) |  | 
| `void` | SetHeadState(`Boolean` positionEnabled, `Boolean` rotationEnabled) |  | 
| `void` | SetHeadWeight(`Single` positionWeight, `Single` rotationWeight) |  | 
| `void` | SetHipsAnchor(`Transform` anchor) |  | 
| `void` | SetHipsState(`Boolean` active) |  | 
| `void` | SetHipsWeight(`Single` active) |  | 
| `void` | SetLocomotionWeight(`Single` weight) |  | 
| `void` | SetLookAtBodyWeight(`Single` weight, `Single` clamp) |  | 
| `void` | SetLookAtEyesWeight(`Single` weight, `Single` clamp) |  | 
| `void` | SetLookAtHeadWeight(`Single` weight, `Single` clamp) |  | 
| `void` | SetLookAtTarget(`Transform` anchor) |  | 
| `void` | SetLookAtWeight(`Single` weight) |  | 
| `void` | SetShoulderAnchor(`Side` side, `Transform` anchor) |  | 
| `void` | SetShoulderState(`Side` side, `Boolean` positionEnabled, `Boolean` rotationEnabled) |  | 
| `void` | SetShoulderWeight(`Side` side, `Single` positionWeight, `Single` rotationWeight) |  | 
| `void` | Setup() |  | 
| `void` | Update() |  | 
| `void` | UpdateBodyRotation() |  | 


## `IKControllerFIK`

```csharp
public class ThunderRoad.IKControllerFIK
    : IkController

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BipedIKCustom` | bipedIk |  | 
| `FullBodyBipedIK` | fullBodyBipedIk |  | 
| `HandPoser` | handPoserLeft |  | 
| `HandPoser` | handPoserRight |  | 
| `FBBIKHeadEffector` | headEffector |  | 
| `Single` | headTorsoBendWeightMultiplier |  | 
| `FingerRig` | leftFingerRig |  | 
| `FingerRig` | rightFingerRig |  | 
| `AnimationCurve` | stretchArmsCurve |  | 
| `AnimationCurve` | stretchLegsCurve |  | 
| `VRIK` | vrik |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Transform` | AddFingerTip(`Transform` bone, `Single` tipDistance) |  | 
| `void` | AddLocomotionDeltaPosition(`Vector3` delta) |  | 
| `void` | AddLocomotionDeltaRotation(`Quaternion` delta, `Vector3` pivot) |  | 
| `FootBoneTarget` | GetFootBoneTarget() |  | 
| `Single` | GetHandPositionWeight(`Side` side) |  | 
| `Single` | GetHandRotationWeight(`Side` side) |  | 
| `Single` | GetHeadWeight() |  | 
| `Single` | GetHipsWeight() |  | 
| `Single` | GetLocomotionWeight() |  | 
| `Single` | GetLookAtWeight() |  | 
| `void` | RefreshState() |  | 
| `void` | SetFootAnchor(`Side` side, `Transform` anchor, `Quaternion` toesRotation) |  | 
| `void` | SetFootPull(`Side` side, `Single` value) |  | 
| `void` | SetFootState(`Side` side, `Boolean` active) |  | 
| `void` | SetFootWeight(`Side` side, `Single` positionWeight, `Single` rotationWeight) |  | 
| `void` | SetFullbody(`Boolean` active) |  | 
| `void` | SetHandAnchor(`Side` side, `Transform` anchor, `Quaternion` palmRotation) |  | 
| `void` | SetHandState(`Side` side, `Boolean` positionEnabled, `Boolean` rotationEnabled) |  | 
| `void` | SetHandWeight(`Side` side, `Single` positionWeight, `Single` rotationWeight) |  | 
| `void` | SetHeadAnchor(`Transform` anchor) |  | 
| `void` | SetHeadState(`Boolean` positionEnabled, `Boolean` rotationEnabled) |  | 
| `void` | SetHeadWeight(`Single` positionWeight, `Single` rotationWeight) |  | 
| `void` | SetHipsAnchor(`Transform` anchor) |  | 
| `void` | SetHipsState(`Boolean` enabled) |  | 
| `void` | SetHipsWeight(`Single` value) |  | 
| `void` | SetLocomotionWeight(`Single` weight) |  | 
| `void` | SetLookAtBodyWeight(`Single` weight, `Single` clamp) |  | 
| `void` | SetLookAtEyesWeight(`Single` weight, `Single` clamp) |  | 
| `void` | SetLookAtHeadWeight(`Single` weight, `Single` clamp) |  | 
| `void` | SetLookAtTarget(`Transform` target) |  | 
| `void` | SetLookAtWeight(`Single` weight) |  | 
| `void` | SetShoulderAnchor(`Side` side, `Transform` anchor) |  | 
| `void` | SetShoulderState(`Side` side, `Boolean` positionEnabled, `Boolean` rotationEnabled) |  | 
| `void` | SetShoulderWeight(`Side` side, `Single` positionWeight, `Single` rotationWeight) |  | 
| `void` | SetState(`State` state) |  | 
| `void` | Setup() |  | 


## `Imbue`

```csharp
public class ThunderRoad.Imbue
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `ColliderGroup` | colliderGroup |  | 
| `Single` | energy |  | 
| `Single` | maxEnergy |  | 
| `SpellCastCharge` | spellCastBase |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `Boolean` | CanConsume(`Single` energyToConsume) |  | 
| `void` | ConsumeInstant(`Single` energyConsumed) |  | 
| `void` | OnCollisionStart(`CollisionInstance` collisionInstance) |  | 
| `void` | OnCollisionStop(`CollisionInstance` collisionInstance) |  | 
| `void` | OnCrystalUse(`Side` side, `Boolean` active) |  | 
| `void` | Start() |  | 
| `void` | Transfer(`SpellCastCharge` spellCastBase, `Single` energyTransfered) |  | 
| `void` | Transfer(`Single` energyTransfered) |  | 
| `void` | Update() |  | 
| `void` | UpdateModule() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | infiniteImbue |  | 
| `Single` | moduleUpdateRate |  | 


## `InputBase`

```csharp
public class ThunderRoad.InputBase

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Enable(`Boolean` active) |  | 
| `void` | FixedUpdate() |  | 
| `Vector3` | GetFootPosition(`Side` side) |  | 
| `Quaternion` | GetFootRotation(`Side` side) |  | 
| `Boolean` | GetFootTracking(`Side` side) |  | 
| `Vector3` | GetFootVelocity(`Side` side) |  | 
| `Vector3[]` | GetHandBonePositions(`Side` side) |  | 
| `Quaternion[]` | GetHandBoneRotations(`Side` side) |  | 
| `Vector3` | GetHandVelocity(`Side` side) |  | 
| `Vector3` | GetWaistPosition() |  | 
| `Quaternion` | GetWaistRotation() |  | 
| `Boolean` | GetWaistTracking() |  | 
| `Vector3` | GetWaistVelocity() |  | 
| `void` | Haptic(`Side` side, `Single` intensity, `Single` frequency) |  | 
| `void` | LateUpdate() |  | 
| `void` | Update() |  | 


## `InputKeyboard`

```csharp
public class ThunderRoad.InputKeyboard
    : InputBase

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | enabled |  | 
| `Single` | rotationSpeed |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Enable(`Boolean` active) |  | 
| `void` | Update() |  | 


## `InputOculus`

```csharp
public class ThunderRoad.InputOculus
    : InputBase

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | analogThreshold |  | 
| `Boolean` | enabled |  | 
| `HapticCapabilities` | hapticCapabilitiesLeft |  | 
| `HapticCapabilities` | hapticCapabilitiesRight |  | 
| `InputDevice` | inputDeviceLeft |  | 
| `InputDevice` | inputDeviceRight |  | 
| `Boolean` | inputFocused |  | 
| `Single` | maxThumbCurlOnGrip |  | 
| `Single` | minFingerCurl |  | 
| `Single` | minGripForMaxThumbCurl |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Enable(`Boolean` active) |  | 
| `void` | FixedUpdate() |  | 
| `Vector3` | GetHandVelocity(`Side` side) |  | 
| `void` | Haptic(`Side` side, `Single` intensity, `Single` frequency) |  | 
| `void` | Update() |  | 


## `InputSteamVR`

```csharp
public class ThunderRoad.InputSteamVR
    : InputBase

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `SteamVR_ActionSet` | actionSet |  | 
| `SteamVR_Action_Boolean` | alternateUse2Action |  | 
| `SteamVR_Action_Single` | alternateUseAction |  | 
| `Single` | analogThreshold |  | 
| `SteamVR_Action_Single` | castAction |  | 
| `SteamVR_Action_Boolean` | clickUiAction |  | 
| `SteamVR_Action_Boolean` | externalViewAction |  | 
| `SteamVR_Action_Boolean` | externalViewLockAction |  | 
| `SteamVR_Input_Sources` | forSources |  | 
| `SteamVR_Action_Boolean` | grabGripAction |  | 
| `SteamVR_Action_Boolean` | grabPinchAction |  | 
| `SteamVR_Action_Vibration` | hapticAction |  | 
| `SteamVR_Action_Vector2` | heightAction |  | 
| `Single` | indexCurlTrigger |  | 
| `SteamVR_Action_Boolean` | jumpAction |  | 
| `SteamVR_Action_Boolean` | kickAction |  | 
| `SteamVR_Action_Boolean` | menuAction |  | 
| `Single` | minFingerCurl |  | 
| `SteamVR_Action_Vector2` | moveAction |  | 
| `SteamVR_Action_Boolean` | movePressAction |  | 
| `SteamVR_Action_Pose` | poseAction |  | 
| `SteamVR_Action_Boolean` | screenshotAction |  | 
| `SteamVR_Action_Vector2` | scrollUiAction |  | 
| `SteamVR_Action_Skeleton` | skeletonLeftAction |  | 
| `SteamVR_Action_Skeleton` | skeletonRightAction |  | 
| `SteamVR_Action_Boolean` | slowTimeAction |  | 
| `SteamVR_Action_Boolean` | spellSelectorAction |  | 
| `SteamVR_Action_Boolean` | telekinesisAction |  | 
| `SteamVR_Action_Vector2` | telekinesisAxisAction |  | 
| `SteamVR_Action_Single` | telekinesisPullAction |  | 
| `SteamVR_Action_Boolean` | telekinesisRepel2Action |  | 
| `SteamVR_Action_Single` | telekinesisRepelAction |  | 
| `SteamVR_Action_Boolean` | telekinesisSpinAction |  | 
| `SteamVR_Action_Vector2` | turnAction |  | 
| `SteamVR_Action_Boolean` | turnPressAction |  | 
| `SteamVR_Action_Single` | useAction |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Enable(`Boolean` active) |  | 
| `void` | FixedUpdate() |  | 
| `Vector3` | GetFootPosition(`Side` side) |  | 
| `Quaternion` | GetFootRotation(`Side` side) |  | 
| `Boolean` | GetFootTracking(`Side` side) |  | 
| `Vector3` | GetFootVelocity(`Side` side) |  | 
| `Vector3[]` | GetHandBonePositions(`Side` side) |  | 
| `Quaternion[]` | GetHandBoneRotations(`Side` side) |  | 
| `Vector3` | GetHandVelocity(`Side` side) |  | 
| `Side` | GetSide(`SteamVR_Input_Sources` steamVR_Input_Sources) |  | 
| `Vector3` | GetWaistPosition() |  | 
| `Quaternion` | GetWaistRotation() |  | 
| `Boolean` | GetWaistTracking() |  | 
| `Vector3` | GetWaistVelocity() |  | 
| `void` | Haptic(`Side` side, `Single` intensity, `Single` frequency) |  | 
| `void` | LateUpdate() |  | 
| `void` | OnBeforeRender() |  | 
| `void` | OnQuit(`VREvent_t` vrEvent) |  | 
| `void` | Update() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | lastFrameCount |  | 


## `InputXR`

```csharp
public class ThunderRoad.InputXR
    : InputBase

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | enabled |  | 
| `Boolean` | inputFocused |  | 
| `Controller` | leftController |  | 
| `Single` | maxThumbCurlOnGrip |  | 
| `Single` | minFingerCurl |  | 
| `Single` | minGripForMaxThumbCurl |  | 
| `Controller` | rightController |  | 
| `Single` | triggerAndGripThreshold |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Enable(`Boolean` active) |  | 
| `Controller` | GetController(`Side` side) |  | 
| `Vector3` | GetHandVelocity(`Side` side) |  | 
| `void` | Haptic(`Side` side, `Single` intensity, `Single` frequency) |  | 
| `void` | Update() |  | 
| `void` | UpdateFingers(`Controller` controller, `Hand` playerControlHand) |  | 


## `Interactable`

```csharp
public class ThunderRoad.Interactable
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `HandSide` | allowedHandSide |  | 
| `Single` | axisLength |  | 
| `InteractableData` | data |  | 
| `Boolean` | initialized |  | 
| `String` | interactableId |  | 
| `Vector3` | touchCenter |  | 
| `Collider` | touchCollider |  | 
| `Single` | touchRadius |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `Boolean` | CanTouch(`RagdollHand` ragdollHand) |  | 
| `InteractionResult` | CheckInteraction(`RagdollHand` ragdollHand) |  | 
| `List<ValueDropdownItem<String>>` | GetAllInteractableID() |  | 
| `void` | HapticRumble(`PlayerHand` playerHand) |  | 
| `void` | Load(`InteractableData` interactableData) |  | 
| `void` | OnDrawGizmosSelected() |  | 
| `void` | OnTouchEnd(`RagdollHand` ragdollHand) |  | 
| `void` | OnTouchStart(`RagdollHand` ragdollHand) |  | 
| `void` | OnTouchStay(`RagdollHand` ragdollHand) |  | 
| `void` | SetTouch(`Boolean` active) |  | 
| `void` | ShowHint(`RagdollHand` ragdollHand) |  | 
| `void` | Start() |  | 
| `void` | TryLoadFromID() |  | 
| `Boolean` | TryTouchAction(`RagdollHand` ragdollHand, `Action` action) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | showTouchHighlighter |  | 


## `InteractableData`

```csharp
public class ThunderRoad.InteractableData
    : CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | disableTouch |  | 
| `String` | highlightDefaultDesignation |  | 
| `String` | highlightDefaultTitle |  | 
| `Boolean` | highlighterViewHandFreeOnly |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | GetCurrentVersion() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | highlighterProximityDistance |  | 
| `Boolean` | showHudHighlighter |  | 
| `Boolean` | showTouchHighlighter |  | 


## `IntroLogo`

```csharp
public class ThunderRoad.IntroLogo
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Camera` | cam |  | 
| `UniversalAdditionalCameraData` | cameraData |  | 
| `Single` | duration |  | 
| `UnityEvent` | endEvent |  | 
| `Single` | fadeDuration |  | 
| `GameObject` | logo |  | 
| `GameObject` | logoHDR |  | 
| `Transform` | logoRoot |  | 
| `Boolean` | running |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Play() |  | 


## `Item`

```csharp
public class ThunderRoad.Item
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<HolderPoint>` | additionalHolderPoints |  | 
| `AsyncOperationHandle<GameObject>` | addressableHandle |  | 
| `AudioContainer` | audioContainerSnap |  | 
| `AudioSource` | audioSource |  | 
| `List<Holder>` | childHolders |  | 
| `List<ColliderGroup>` | colliderGroups |  | 
| `List<CollisionHandler>` | collisionHandlers |  | 
| `Single` | creaturePhysicToggleRadius |  | 
| `Single` | cullingDetectionCycleSpeed |  | 
| `Single` | cullingDetectionCycleTime |  | 
| `Boolean` | cullingDetectionEnabled |  | 
| `Room` | currentRoom |  | 
| `Vector3` | customCenterOfMass |  | 
| `Boolean` | customInertiaTensor |  | 
| `CapsuleCollider` | customInertiaTensorCollider |  | 
| `Vector3` | customInertiaTensorPos |  | 
| `Quaternion` | customInertiaTensorRot |  | 
| `List<CustomReference>` | customReferences |  | 
| `List<CustomSnap>` | customSnaps |  | 
| `ItemData` | data |  | 
| `Boolean` | disableSnap |  | 
| `Boolean` | disallowDespawn |  | 
| `Boolean` | disallowRoomDespawn |  | 
| `Single` | distantGrabSafeDistance |  | 
| `Boolean` | distantGrabSpinEnabled |  | 
| `Single` | distantGrabThrowRatio |  | 
| `List<HingeEffect>` | effectHinges |  | 
| `Transform` | flyDirRef |  | 
| `Boolean` | flyFromThrow |  | 
| `Single` | flyRotationSpeed |  | 
| `Single` | flyThrowAngle |  | 
| `Boolean` | handlerArmGrabbed |  | 
| `List<RagdollHand>` | handlers |  | 
| `List<Handle>` | handles |  | 
| `Boolean` | hanging |  | 
| `Holder` | holder |  | 
| `Transform` | holderPoint |  | 
| `Collider` | ignoredCollider |  | 
| `Item` | ignoredItem |  | 
| `Ragdoll` | ignoredRagdoll |  | 
| `List<Imbue>` | imbues |  | 
| `Boolean` | isCulled |  | 
| `Boolean` | isFlying |  | 
| `Boolean` | isGripped |  | 
| `Boolean` | isPenetrating |  | 
| `Boolean` | isPooled |  | 
| `Boolean` | isTelekinesisGrabbed |  | 
| `Boolean` | isThrowed |  | 
| `String` | itemId |  | 
| `RagdollHand` | lastHandler |  | 
| `Single` | lastInteractionTime |  | 
| `RagdollHand` | leftNpcHand |  | 
| `PlayerHand` | leftPlayerHand |  | 
| `LightVolumeReceiver` | lightVolumeReceiver |  | 
| `Boolean` | loaded |  | 
| `List<ItemMagnet>` | magnets |  | 
| `CollisionHandler` | mainCollisionHandler |  | 
| `Handle` | mainHandleLeft |  | 
| `RagdollHand` | mainHandler |  | 
| `Handle` | mainHandleRight |  | 
| `Single` | orgMass |  | 
| `Single` | orgSleepThreshold |  | 
| `Boolean` | parryActive |  | 
| `Transform` | parryPoint |  | 
| `List<ParryTarget>` | parryTargets |  | 
| `Preview` | preview |  | 
| `Rigidbody` | rb |  | 
| `List<Renderer>` | renderers |  | 
| `List<RevealDecal>` | revealDecals |  | 
| `RagdollHand` | rightNpcHand |  | 
| `PlayerHand` | rightPlayerHand |  | 
| `List<SavedValue>` | savedValues |  | 
| `Single` | snapPitchRange |  | 
| `Single` | spawnTime |  | 
| `List<SpellCaster>` | tkHandlers |  | 
| `Boolean` | updateReveal |  | 
| `Boolean` | useCustomCenterOfMass |  | 
| `List<WhooshPoint>` | whooshPoints |  | 
| `Zone` | zone |  | 


Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `CullEvent` | OnCullEvent |  | 
| `DamageReceivedDelegate` | OnDamageReceivedEvent |  | 
| `LoadDelegate` | OnDataLoaded |  | 
| `SpawnEvent` | OnDespawnEvent |  | 
| `ThrowingDelegate` | OnFlyEndEvent |  | 
| `ThrowingDelegate` | OnFlyStartEvent |  | 
| `GrabDelegate` | OnGrabEvent |  | 
| `HeldActionDelegate` | OnHeldActionEvent |  | 
| `MagnetDelegate` | OnMagnetCatchEvent |  | 
| `MagnetDelegate` | OnMagnetReleaseEvent |  | 
| `HolderDelegate` | OnSnapEvent |  | 
| `SpawnEvent` | OnSpawnEvent |  | 
| `TelekinesisDelegate` | OnTelekinesisGrabEvent |  | 
| `TelekinesisDelegate` | OnTelekinesisReleaseEvent |  | 
| `TouchActionDelegate` | OnTouchActionEvent |  | 
| `ReleaseDelegate` | OnUngrabEvent |  | 
| `HolderDelegate` | OnUnSnapEvent |  | 
| `ZoneEvent` | OnZoneEvent |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | CalculateCustomInertiaTensor() |  | 
| `void` | CheckDestroyedMeshRenderers() |  | 
| `void` | Despawn(`Single` delay) |  | 
| `void` | Despawn() |  | 
| `void` | ForceMainHandler(`RagdollHand` ragdollHand) |  | 
| `List<ValueDropdownItem<String>>` | GetAllItemID() |  | 
| `Transform` | GetCustomReference(`String` name) |  | 
| `HolderPoint` | GetDefaultHolderPoint() |  | 
| `HolderPoint` | GetHolderPoint(`String` holderPoint) |  | 
| `Handle` | GetMainHandle(`Side` side) |  | 
| `void` | Hide(`Boolean` hide) |  | 
| `void` | IgnoreColliderCollision(`Collider` targetCollider) |  | 
| `void` | IgnoreObjectCollision(`Item` item) |  | 
| `void` | IgnoreRagdollCollision(`Ragdoll` ragdoll) |  | 
| `void` | IgnoreRagdollCollision(`Ragdoll` ragdoll, `Type` ignoredParts = 0) |  | 
| `void` | InvokeMagnetCatchEvent(`ItemMagnet` itemMagnet, `EventTime` eventTime) |  | 
| `void` | InvokeMagnetReleaseEvent(`ItemMagnet` itemMagnet, `EventTime` eventTime) |  | 
| `void` | InvokeOnSpawnEvent(`EventTime` eventTime) |  | 
| `Boolean` | IsHanded(`Side` side) |  | 
| `Boolean` | IsHanded(`Handle` ignoreHandle = null) |  | 
| `Boolean` | IsTwoHanded(`List<Handle>` validHandles = null) |  | 
| `Boolean` | IsVisible() |  | 
| `void` | Load(`ItemData` itemData) |  | 
| `void` | OnCollisionStartEvent(`CollisionInstance` collisionInstance) |  | 
| `void` | OnDamageReceived(`CollisionInstance` collisionInstance) |  | 
| `void` | OnDisable() |  | 
| `void` | OnDrawGizmosSelected() |  | 
| `void` | OnEnable() |  | 
| `void` | OnGrab(`Handle` handle, `RagdollHand` ragdollHand) |  | 
| `void` | OnHeldAction(`RagdollHand` ragdollHand, `Handle` handle, `Action` action) |  | 
| `void` | OnSnap(`Holder` holder, `Boolean` silent = False) |  | 
| `void` | OnTelekinesisGrab(`Handle` handle, `SpellTelekinesis` teleGrabber) |  | 
| `void` | OnTelekinesisRelease(`Handle` handle, `SpellTelekinesis` teleGrabber) |  | 
| `void` | OnTouchAction(`Interactable` interactable, `Action` action) |  | 
| `void` | OnUnGrab(`Handle` handle, `RagdollHand` ragdollHand, `Boolean` throwing) |  | 
| `void` | OnUnSnap(`Holder` holder, `Boolean` silent = False) |  | 
| `void` | OnValidate() |  | 
| `void` | RefreshAllowTelekinesis() |  | 
| `void` | RefreshCollision(`Boolean` throwing = False) |  | 
| `void` | RefreshCollisionTest() |  | 
| `void` | ResetCenterOfMass() |  | 
| `void` | ResetColliderCollision() |  | 
| `void` | ResetInertiaTensor() |  | 
| `void` | ResetObjectCollision() |  | 
| `void` | ResetRagdollCollision() |  | 
| `void` | SetCenterOfMass(`Vector3` localPosition) |  | 
| `void` | SetColliderAndMeshLayer(`Int32` layer) |  | 
| `void` | SetColliderLayer(`Int32` layer) |  | 
| `void` | SetCull(`Boolean` cull) |  | 
| `void` | SetCustomInertiaTensor() |  | 
| `void` | SetMeshLayer(`Int32` layer) |  | 
| `void` | SetParryMagic(`Boolean` active) |  | 
| `void` | SetSavedValue(`String` id, `String` value) |  | 
| `void` | Start() |  | 
| `void` | StopFlying() |  | 
| `void` | StopThrowing() |  | 
| `void` | Throw(`Single` throwMultiplier = 1, `FlyDetection` flyDetection = CheckAngle) |  | 
| `Boolean` | TryGetSavedValue(`String` id, `String&` value) |  | 
| `void` | Update() |  | 
| `void` | UpdateReveal() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Item>` | all |  | 
| `List<Item>` | allActive |  | 
| `List<Item>` | allHanging |  | 
| `List<Item>` | allThrowed |  | 
| `List<Item>` | allTk |  | 
| `String` | parryMagicTag |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DrawGizmoArrow(`Vector3` pos, `Vector3` direction, `Vector3` upwards, `Color` color, `Single` arrowHeadLength = 0.25, `Single` arrowHeadAngle = 20) |  | 


## `ItemData`

```csharp
public class ThunderRoad.ItemData
    : CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | androidPooledCount |  | 
| `Single` | angularDrag |  | 
| `String` | author |  | 
| `String[]` | categoryPath |  | 
| `List<ColliderGroup>` | colliderGroups |  | 
| `Boolean` | collisionEnterOnly |  | 
| `Int32` | collisionMaxOverride |  | 
| `Boolean` | collisionNoMinVelocityCheck |  | 
| `List<CustomSnap>` | customSnaps |  | 
| `List<Damager>` | damagers |  | 
| `String` | description |  | 
| `String` | displayName |  | 
| `Single` | drag |  | 
| `List<EffectHinge>` | effectHinges |  | 
| `Boolean` | flyFromThrow |  | 
| `Single` | flyRotationSpeed |  | 
| `Single` | flyThrowAngle |  | 
| `LayerName` | forceLayer |  | 
| `Boolean` | grabAndGripClimb |  | 
| `Boolean` | grippable |  | 
| `Texture` | icon |  | 
| `String` | iconAddress |  | 
| `List<IconMarker>` | iconDamagerMarkers |  | 
| `EffectData` | iconEffectData |  | 
| `String` | iconEffectId |  | 
| `IResourceLocation` | iconLocation |  | 
| `List<Interactable>` | Interactables |  | 
| `Boolean` | isStackable |  | 
| `Int32` | levelRequired |  | 
| `String` | localizationId |  | 
| `Single` | manaRegenMultiplier |  | 
| `Single` | mass |  | 
| `ItemModuleAI` | moduleAI |  | 
| `List<ItemModule>` | modules |  | 
| `Boolean` | playerGrabAndGripChangeLayer |  | 
| `Int32` | pooledCount |  | 
| `GameObject` | prefab |  | 
| `String` | prefabAddress |  | 
| `IResourceLocation` | prefabLocation |  | 
| `Single` | price |  | 
| `Boolean` | purchasable |  | 
| `String` | slot |  | 
| `String` | snapAudioContainerAddress |  | 
| `IResourceLocation` | snapAudioContainerLocation |  | 
| `Single` | spellChargeSpeedNPCMultiplier |  | 
| `Single` | spellChargeSpeedPlayerMultiplier |  | 
| `Single` | telekinesisSafeDistance |  | 
| `Boolean` | telekinesisSpinEnabled |  | 
| `Single` | telekinesisThrowRatio |  | 
| `Int32` | tier |  | 
| `String` | tierString |  | 
| `Type` | type |  | 
| `List<Whoosh>` | whooshs |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<ValueDropdownItem<String>>` | GetAllEffectID() |  | 
| `List<ValueDropdownItem<String>>` | GetAllHolderSlots() |  | 
| `List<ValueDropdownItem<String>>` | GetCategories() |  | 
| `Int32` | GetCurrentVersion() |  | 
| `T` | GetModule() |  | 
| `Int32` | GetPooledCount() |  | 
| `Boolean` | HasModule() |  | 
| `IEnumerator` | LoadAddressableAssetsCoroutine() |  | 
| `void` | LoadIconAsync(`Action<Texture>` callback) |  | 
| `void` | LoadPrefabAsync(`Action<Item>` callback) |  | 
| `IEnumerator` | LoadPrefabCoroutine(`Action<Item>` callback) |  | 
| `void` | OnCatalogRefresh() |  | 
| `IEnumerator` | OnCatalogRefreshCoroutine() |  | 
| `void` | ReleaseAddressableAssets() |  | 
| `void` | Rename(`String` newName) |  | 
| `void` | SpawnAsync(`Action<Item>` callback, `Nullable<Vector3>` position = null, `Nullable<Quaternion>` rotation = null, `Transform` parent = null, `Boolean` pooled = True, `List<SavedValue>` savedValues = null) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | itemIndex |  | 
| `Transform` | poolRoot |  | 
| `List<Pool>` | pools |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ClearPool() |  | 
| `void` | DespawnAllPooled() |  | 
| `IEnumerator` | GeneratePool() |  | 
| `void` | ItemInstantiateCallback(`Item` item, `Pool` pool) |  | 
| `void` | ReturnToPool(`Item` item) |  | 


## `ItemMagicProjectile`

```csharp
public class ThunderRoad.ItemMagicProjectile
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | allowDeflect |  | 
| `EffectData` | deflectEffectData |  | 
| `EffectInstance` | effectInstance |  | 
| `Boolean` | guided |  | 
| `Vector3` | guidedDirection |  | 
| `Single` | imbueEnergyTransfered |  | 
| `SpellCastCharge` | imbueSpellCastCharge |  | 
| `Item` | item |  | 
| `ItemModuleMagicProjectile` | module |  | 
| `Item` | shooter |  | 
| `Single` | speed |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | Despawn() |  | 
| `void` | Fire(`Vector3` velocity, `EffectData` effectData, `Item` shooterItem = null, `Ragdoll` shooterRagdoll = null) |  | 
| `void` | FixedUpdate() |  | 
| `void` | OnCollision(`CollisionInstance` collisionInstance) |  | 
| `void` | OnEffectFinished(`EffectInstance` effectInstance) |  | 
| `void` | ResetCollision() |  | 
| `void` | Start() |  | 


## `ItemMagnet`

```csharp
public class ThunderRoad.ItemMagnet
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | autoUngrab |  | 
| `List<CapturedItem>` | capturedItems |  | 
| `Single` | gravityRatio |  | 
| `Int32` | maxCount |  | 
| `Single` | positionDamper |  | 
| `Single` | positionMaxForce |  | 
| `Single` | positionSpring |  | 
| `Rigidbody` | rb |  | 
| `Single` | rotationDamper |  | 
| `Single` | rotationMaxForce |  | 
| `Single` | rotationSpring |  | 
| `Single` | sleepThresholdRatio |  | 
| `List<String>` | slots |  | 
| `Single` | stabilizedMaxAngle |  | 
| `Single` | stabilizedMaxDistance |  | 
| `Single` | stabilizedMaxUpAngle |  | 
| `FilterLogic` | tagFilter |  | 
| `Collider` | trigger |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `List<ValueDropdownItem<String>>` | GetAllHolderSlots() |  | 
| `Boolean` | ItemAllowed(`Item` item) |  | 
| `void` | OnItemCatch(`Item` item, `EventTime` eventTime) |  | 
| `void` | OnItemRelease(`Item` item, `EventTime` eventTime) |  | 
| `void` | OnTriggerEnter(`Collider` other) |  | 
| `void` | OnTriggerExit(`Collider` other) |  | 
| `void` | OnValidate() |  | 
| `void` | RefreshJoints() |  | 
| `Boolean` | SlotAllowed(`String` slot) |  | 
| `void` | Update() |  | 


## `ItemModule`

```csharp
public class ThunderRoad.ItemModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Item` | item |  | 
| `ItemData` | itemData |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | type |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `IEnumerator` | LoadAddressableAssetsCoroutine(`ItemData` data) |  | 
| `void` | OnItemDataRefresh(`ItemData` data) |  | 
| `void` | OnItemLoaded(`Item` item) |  | 
| `void` | ReleaseAddressableAssets() |  | 


## `ItemModuleAI`

```csharp
public class ThunderRoad.ItemModuleAI
    : ItemModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | allowDynamicHeight |  | 
| `Single` | armResistanceMultiplier |  | 
| `Boolean` | attackForceParryIgnoreRotation |  | 
| `Boolean` | attackIgnore |  | 
| `Boolean` | defenseHasPriority |  | 
| `Vector3` | parryDefaultLeftRotation |  | 
| `Vector3` | parryDefaultPosition |  | 
| `Vector3` | parryDefaultRightRotation |  | 
| `Single` | parryDualRotation |  | 
| `Boolean` | parryIgnoreRotation |  | 
| `Vector2` | parryRevertAngleRange |  | 
| `Single` | parryRotation |  | 
| `WeaponClass` | weaponClass |  | 
| `WeaponHandling` | weaponHandling |  | 


## `ItemModuleBow`

```csharp
public class ThunderRoad.ItemModuleBow
    : ItemModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | arrowProjectileID |  | 
| `Single` | audioDrawPullSpeed |  | 
| `String` | audioGroupDrawAddress |  | 
| `String` | audioGroupShootAddress |  | 
| `Single` | audioShootMinPull |  | 
| `String` | audioStringAddress |  | 
| `Boolean` | autoSpawnArrow |  | 
| `Single` | baseShootVelocity |  | 
| `Single` | stringSpring |  | 
| `Single` | velocityMultiplier |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<ValueDropdownItem<String>>` | GetAllEffectID() |  | 
| `List<ValueDropdownItem<String>>` | GetAllItemID() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | forceAutoSpawnArrow |  | 


## `ItemModuleMagicProjectile`

```csharp
public class ThunderRoad.ItemModuleMagicProjectile
    : ItemModule

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnItemLoaded(`Item` item) |  | 


## `ItemModulePotion`

```csharp
public class ThunderRoad.ItemModulePotion
    : ItemModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `LayerMask` | collisionLayer |  | 
| `List<Content>` | contents |  | 
| `String` | effectFlowId |  | 
| `Single` | flowMaxAngle |  | 
| `Single` | flowMinAngle |  | 
| `Single` | flowSpeed |  | 
| `Single` | maxLevel |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<ValueDropdownItem<String>>` | GetAllEffectID() |  | 
| `List<ValueDropdownItem<String>>` | GetAllItemID() |  | 
| `void` | OnItemLoaded(`Item` item) |  | 


## `ItemModuleSpell`

```csharp
public class ThunderRoad.ItemModuleSpell
    : ItemModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `SpellData` | spellData |  | 
| `String` | spellId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<ValueDropdownItem<String>>` | GetAllSpellID() |  | 
| `void` | OnItemDataRefresh(`ItemData` data) |  | 


## `ItemModuleWardrobe`

```csharp
public class ThunderRoad.ItemModuleWardrobe
    : ItemModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `WardRobeCategory` | category |  | 
| `List<CreatureWardrobe>` | wardrobes |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `CreatureWardrobe` | GetWardrobe(`Creature` creature) |  | 
| `Boolean` | IsCompatible(`Creature` creature) |  | 
| `IEnumerator` | LoadAddressableAssetsCoroutine(`ItemData` data) |  | 
| `void` | ReleaseAddressableAssets() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Dictionary<String, String[]>` | locations |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | GetLayer(`String` channel, `String` layer) |  | 


## `ItemPreview`

```csharp
public class ThunderRoad.ItemPreview
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Texture>` | addressableTextures |  | 
| `GameObject` | detailPage |  | 
| `GameObject` | iconDamagerPrefab |  | 
| `GameObject` | noSelectionPage |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnEnable() |  | 


## `ItemSpawner`

```csharp
public class ThunderRoad.ItemSpawner
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | disallowDespawn |  | 
| `String` | itemId |  | 
| `Boolean` | pooled |  | 
| `Boolean` | spawnOnStart |  | 
| `Transform` | spawnPoint |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<ValueDropdownItem<String>>` | GetAllItemID() |  | 
| `void` | Spawn() |  | 
| `void` | Start() |  | 


## `JsonMergeKeyAttribute`

```csharp
public class ThunderRoad.JsonMergeKeyAttribute
    : Attribute, _Attribute

```

## `KeyedListMergeConverter`

```csharp
public class ThunderRoad.KeyedListMergeConverter
    : JsonConverter

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CanWrite |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CanConvert(`Type` objectType) |  | 
| `Object` | ReadJson(`JsonReader` reader, `Type` objectType, `Object` existingValue, `JsonSerializer` serializer) |  | 
| `void` | WriteJson(`JsonWriter` writer, `Object` value, `JsonSerializer` serializer) |  | 


## `LadderBuilder`

```csharp
public class ThunderRoad.LadderBuilder
    : MonoBehaviour

```

## `LayerName`

```csharp
public enum ThunderRoad.LayerName
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | None |  | 
| `1` | Default |  | 
| `2` | PlayerLocomotion |  | 
| `3` | BodyLocomotion |  | 
| `4` | Touch |  | 
| `5` | MovingItem |  | 
| `6` | DroppedItem |  | 
| `7` | ItemAndRagdollOnly |  | 
| `8` | TouchObject |  | 
| `9` | Avatar |  | 
| `10` | NPC |  | 
| `11` | FPVHide |  | 
| `12` | LocomotionOnly |  | 
| `13` | Ragdoll |  | 
| `14` | PostProcess |  | 
| `15` | PlayerHandAndFoot |  | 
| `16` | PlayerLocomotionObject |  | 
| `17` | LiquidFlow |  | 
| `18` | Zone |  | 
| `19` | NoLocomotion |  | 
| `20` | MovingObjectOnly |  | 
| `21` | SkyDome |  | 
| `22` | Highlighter |  | 


## `LayerType`

```csharp
public enum ThunderRoad.LayerType
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | Touch |  | 
| `1` | Body |  | 
| `2` | Ragdoll |  | 
| `3` | Object |  | 
| `4` | Stair |  | 
| `5` | Avatar |  | 
| `6` | AvatarObject |  | 
| `7` | FloatingHand |  | 
| `8` | Damage |  | 
| `9` | Creature |  | 
| `10` | UI |  | 
| `11` | Player |  | 


## `Level`

```csharp
public class ThunderRoad.Level
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<CustomReference>` | customReferences |  | 
| `LevelData` | data |  | 
| `Dungeon` | dungeon |  | 
| `Boolean` | loaded |  | 
| `UnityEvent` | loadedEvent |  | 
| `Mode` | mode |  | 
| `Dictionary<String, Double>` | options |  | 
| `Color` | originalFogColor |  | 
| `Color` | originalShadowColor |  | 
| `Transform` | playerStart |  | 
| `State` | state |  | 


Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `LevelLoadedEvent` | OnLevelEvent |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `Int32` | GetDifficulty() |  | 
| `IEnumerator` | OnLevelLoadCoroutine(`LevelData` levelData, `Mode` levelMode = null, `Dictionary<String, Double>` levelOptions = null) |  | 
| `void` | OnLevelUnload() |  | 
| `Boolean` | TryGetCurrentDifficultyMultipliers(`DifficultyMultipliers&` difficultyMultipliers) |  | 
| `void` | Update() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Level` | current |  | 
| `Level` | master |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ChangeLightMapMode(`LightmapsMode` lightmapsMode) |  | 
| `void` | CheckLightMapMode() |  | 
| `void` | TetrahedralizeLightProbes() |  | 


## `LevelData`

```csharp
public class ThunderRoad.LevelData
    : CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<CustomCameras>` | customCameras |  | 
| `String` | description |  | 
| `String[]` | dungeonFlowAddresses |  | 
| `Boolean` | hideOnAndroid |  | 
| `String` | iconAddress |  | 
| `Texture2D` | iconLoaded |  | 
| `IResourceLocation` | iconLocation |  | 
| `String` | mapIconAddress |  | 
| `String` | mapIconHoverAddress |  | 
| `Texture2D` | mapIconHoverLoaded |  | 
| `Texture2D` | mapIconLoaded |  | 
| `String` | mapId |  | 
| `String` | mapLocation |  | 
| `String` | mapNameDisplay |  | 
| `String` | mapObjectAddress |  | 
| `GameObject` | mapObjectLoaded |  | 
| `String` | mapSketchAddress |  | 
| `Texture2D` | mapSketchLoaded |  | 
| `String` | mapTextureAddress |  | 
| `Texture2D` | mapTextureLoaded |  | 
| `Int32` | modePickCountPerRank |  | 
| `List<Mode>` | modes |  | 
| `String` | name |  | 
| `String` | sceneAddress |  | 
| `IResourceLocation` | sceneLocation |  | 
| `Boolean` | showInLevelSelection |  | 
| `Boolean` | showOnMap |  | 
| `Boolean` | spawnBody |  | 
| `Boolean` | spawnPlayer |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | GetCurrentVersion() |  | 
| `Mode` | GetMode(`String` modeName = null) |  | 
| `IEnumerator` | OnCatalogRefreshCoroutine() |  | 


## `LevelModule`

```csharp
public class ThunderRoad.LevelModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Level` | level |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | type |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `IEnumerator` | OnLoadCoroutine() |  | 
| `IEnumerator` | OnPlayerSpawnCoroutine() |  | 
| `void` | OnUnload() |  | 
| `void` | Update() |  | 


## `LevelModuleCleaner`

```csharp
public class ThunderRoad.LevelModuleCleaner
    : LevelModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | cleanBodies |  | 
| `Single` | cleanerRate |  | 
| `Single` | lastCleaningTime |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CleanDeadBodies() |  | 
| `void` | CleanDroppedObjects() |  | 
| `void` | Update() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | cleanMaxDeadCount |  | 
| `Int32` | cleanMaxDropCount |  | 
| `Boolean` | cleanVisibleDead |  | 


## `LevelModuleDeath`

```csharp
public class ThunderRoad.LevelModuleDeath
    : LevelModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Behaviour` | behaviour |  | 
| `Single` | delayBeforeLoad |  | 
| `Boolean` | disablePlayerLocomotion |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnCreatureKill(`Creature` creature, `Player` player, `CollisionInstance` collisionInstance, `EventTime` eventTime) |  | 
| `IEnumerator` | OnDeathCoroutine() |  | 
| `IEnumerator` | OnLoadCoroutine() |  | 
| `void` | OnPossessionEvent(`Creature` creature, `EventTime` eventTime) |  | 
| `void` | OnUnload() |  | 


## `LevelModuleLeaderboard`

```csharp
public class ThunderRoad.LevelModuleLeaderboard
    : LevelModule

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnCreatureKill(`Creature` creature, `Player` player, `CollisionInstance` collisionInstance, `EventTime` eventTime) |  | 
| `IEnumerator` | OnLoadCoroutine() |  | 
| `void` | Save(`String` aName) |  | 


## `LevelModuleMusic`

```csharp
public class ThunderRoad.LevelModuleMusic
    : LevelModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | dynamicMusic |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<ValueDropdownItem<String>>` | GetAllMusicID() |  | 
| `IEnumerator` | OnLoadCoroutine() |  | 


## `LevelModulePersistence`

```csharp
public class ThunderRoad.LevelModulePersistence
    : LevelModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | loadGrabbedItems |  | 
| `Boolean` | loadSavedCreatures |  | 
| `String` | locationID |  | 
| `SaveOptions` | saveOnUnload |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `IEnumerator` | OnPlayerSpawnCoroutine() |  | 
| `void` | OnUnload() |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | SaveToPlayerCharacterData(`SaveOptions` saveOptions, `String` locationID = null) |  | 


## `LevelModuleSurvival`

```csharp
public class ThunderRoad.LevelModuleSurvival
    : LevelModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | currentWaveNumberForReward |  | 
| `Single` | delayBetweenWave |  | 
| `Boolean` | disallowHealthPotions |  | 
| `Single` | drivePositionDamper |  | 
| `Single` | drivePositionSpring |  | 
| `String` | firstRewardscontainerID |  | 
| `LevelModuleTutorial` | levelModuleTutorial |  | 
| `Boolean` | repeatLastWaveIndefinitly |  | 
| `List<Item>` | rewards |  | 
| `List<Animator>` | rewardsAnimator |  | 
| `List<GameObject>` | rewardsFX |  | 
| `List<AudioSource>` | rewardsSound |  | 
| `List<Transform>` | rewardsSpawnPosition |  | 
| `Int32` | rewardsToSpawn |  | 
| `Single` | slerpPositionDamper |  | 
| `Single` | slerpPositionSpring |  | 
| `Single` | spawnPositionHeight |  | 
| `Single` | startDelay |  | 
| `String` | textFightId |  | 
| `String` | textGroupId |  | 
| `String` | textNextWaveId |  | 
| `String` | textWaveId |  | 
| `Boolean` | waitingToChooseReward |  | 
| `Coroutine` | waveEndedCoroutine |  | 
| `Int32` | waveIndex |  | 
| `List<Waves>` | waves |  | 
| `Int32` | wavesNumberForReward |  | 
| `WaveSpawner` | waveSpawner |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ChoosenReward(`Transform` aTransform) |  | 
| `List<ValueDropdownItem<String>>` | GetAllContainerID() |  | 
| `List<ValueDropdownItem<String>>` | GetAllTextGroupID() |  | 
| `List<ValueDropdownItem<String>>` | GetAllTextId() |  | 
| `List<ValueDropdownItem<String>>` | GetAllWaveID() |  | 
| `IEnumerator` | OnLoadCoroutine() |  | 
| `void` | OnUnload() |  | 
| `void` | OnWaveEnded() |  | 
| `void` | SpawnRandomItem(`Int32` aNumber, `Boolean` aIsFirst = False) |  | 


## `LevelModuleTutorial`

```csharp
public class ThunderRoad.LevelModuleTutorial
    : LevelModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Coroutine` | coroutine |  | 
| `Single` | delayToStart |  | 
| `Single` | drivePositionDamper |  | 
| `Single` | drivePositionSpring |  | 
| `Boolean` | launchOnStart |  | 
| `List<Animator>` | rewardsAnimator |  | 
| `GameObject` | rewardsFX |  | 
| `Transform` | rewardSpawnPosition |  | 
| `AudioSource` | rewardsSound |  | 
| `String` | safeWeaponReferenceID |  | 
| `Single` | slerpPositionDamper |  | 
| `Single` | slerpPositionSpring |  | 
| `Single` | spawnPositionHeight |  | 
| `String` | tutorialID |  | 
| `String` | uiMaterialAddress |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<ValueDropdownItem<String>>` | GetAllTutorialID() |  | 
| `IEnumerator` | OnLoadCoroutine() |  | 
| `void` | OnUnload() |  | 


## `LevelModuleXP`

```csharp
public class ThunderRoad.LevelModuleXP
    : LevelModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | currentHitReceived |  | 
| `Int32` | currentHonor |  | 
| `Int32` | currentKill |  | 
| `Int32` | currentXP |  | 
| `List<HistoryEvent>` | history |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Action` | GetAction(`Creature` creature, `CollisionInstance` collisionInstance, `Int32&` bonusMalus, `Int32&` honor) |  | 
| `Modifier` | GetModifier(`Creature` creature, `CollisionInstance` collisionInstance, `Int32&` bonusMalus, `Int32&` honor) |  | 
| `Int32` | GetScore() |  | 
| `Scores` | GetScores() |  | 
| `void` | OnCreatureHit(`Creature` creature, `CollisionInstance` collisionInstance) |  | 
| `void` | OnCreatureKill(`Creature` creature, `Player` player, `CollisionInstance` collisionInstance, `EventTime` eventTime) |  | 
| `IEnumerator` | OnLoadCoroutine() |  | 
| `void` | OnUnload() |  | 
| `void` | OnWaveBegin() |  | 
| `void` | OnWaveLoop() |  | 


## `Lever`

```csharp
public class ThunderRoad.Lever
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `CollisionHandler` | collisionHandler |  | 
| `Single` | deadZone |  | 
| `HingeJoint` | joint |  | 
| `Single` | lastAngle |  | 
| `UnityEvent<Single>` | leverAnalogEvent |  | 
| `UnityEvent` | leverDownEvent |  | 
| `UnityEvent` | leverUpEvent |  | 
| `State` | state |  | 


## `LightController`

```csharp
public class ThunderRoad.LightController
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | maxIntensity |  | 
| `Single` | maxRange |  | 
| `Single` | minIntensity |  | 
| `Single` | minRange |  | 
| `Single` | randomRange |  | 
| `Single` | randomRangeIntensity |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | SetActive(`Boolean` active) |  | 
| `void` | SetColor(`Color` mainColor) |  | 
| `void` | SetIntensity(`Single` value) |  | 


## `LightVolumeReceiver`

```csharp
public class ThunderRoad.LightVolumeReceiver
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | addMaterialInstances |  | 
| `Creature` | creature |  | 
| `LightProbeVolume` | currentLightProbeVolume |  | 
| `Boolean` | initRenderersOnStart |  | 
| `Item` | item |  | 
| `List<LightProbeVolume>` | lightProbeVolumes |  | 
| `List<MaterialInstance>` | materialInstances |  | 
| `MaterialPropertyBlock` | materialPropertyBlock |  | 
| `Method` | method |  | 
| `LightVolumeReceiver` | parentReceiver |  | 
| `List<Renderer>` | renderers |  | 
| `VolumeDetection` | volumeDetection |  | 


Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `OnVolumeChangeDelegate` | onVolumeChangeEvent |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnDespawn(`EventTime` eventTime) |  | 
| `void` | OnDungeonGenerated(`EventTime` eventTime) |  | 
| `void` | OnParentVolumeChange(`LightProbeVolume` currentLightProbeVolume, `List<LightProbeVolume>` lightProbeVolumes) |  | 
| `void` | OnRootRagdollPartTriggerEnter(`Collider` other) |  | 
| `void` | OnRootRagdollPartTriggerExit(`Collider` other) |  | 
| `void` | OnSnap(`Holder` holder) |  | 
| `void` | OnTriggerEnter(`Collider` other) |  | 
| `void` | OnTriggerExit(`Collider` other) |  | 
| `void` | OnUnSnap(`Holder` holder) |  | 
| `void` | RestoreRenderers() |  | 
| `void` | SetRenderers(`List<Renderer>` renderers, `Boolean` addMaterialInstances = True) |  | 
| `void` | UpdateRenderers() |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `LightProbeVolume` | ApplyProbeVolume(`Renderer` renderer, `MaterialPropertyBlock` materialPropertyBlock) |  | 
| `void` | DisableProbeVolume(`Renderer` renderer) |  | 
| `LightProbeVolume` | GetVolumeFromPosition(`Vector3` position) |  | 


## `LiquidContainer`

```csharp
public class ThunderRoad.LiquidContainer
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `LayerMask` | collisionLayer |  | 
| `List<Content>` | contents |  | 
| `EffectInstance` | effectFlow |  | 
| `EffectData` | effectFlowData |  | 
| `String` | effectFlowId |  | 
| `Transform` | flow |  | 
| `Single` | flowMaxAngle |  | 
| `Single` | flowMinAngle |  | 
| `Single` | flowSpeed |  | 
| `Boolean` | liquidFlow |  | 
| `Text` | liquidLevelText |  | 
| `Single` | maxLevel |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddLiquid(`LiquidData` liquidData, `Single` level) |  | 
| `void` | Awake() |  | 
| `List<ValueDropdownItem<String>>` | GetAllEffectID() |  | 
| `List<ValueDropdownItem<String>>` | GetAllItemID() |  | 
| `Single` | GetLiquidLevel() |  | 
| `void` | Init(`Item` item) |  | 
| `void` | OnCorkSnapped(`Item` corkItem) |  | 
| `void` | OnCorkUnsnapped(`Item` corkItem) |  | 
| `void` | OnGrab(`Handle` handle, `RagdollHand` ragdollHand) |  | 
| `void` | OnLiquidFlowing() |  | 
| `void` | OnLiquidFlowStart() |  | 
| `void` | OnLiquidFlowStop() |  | 
| `void` | OnRelease(`Handle` handle, `RagdollHand` ragdollHand, `Boolean` forSnap) |  | 
| `void` | SpawnEffectFlowLoop() |  | 
| `void` | Update() |  | 


## `LiquidData`

```csharp
public class ThunderRoad.LiquidData
    : CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Color` | color |  | 
| `String` | designation |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnLiquidReception(`LiquidReceiver` liquidReceiver, `Single` dilution, `LiquidContainer` liquidContainer) |  | 


## `LiquidHealth`

```csharp
public class ThunderRoad.LiquidHealth
    : LiquidData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | healthGain |  | 
| `Single` | revealBlitDuration |  | 
| `Single` | revealBlitStep |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnLiquidReception(`LiquidReceiver` liquidReceiver, `Single` dilution, `LiquidContainer` liquidContainer) |  | 


## `LiquidPoison`

```csharp
public class ThunderRoad.LiquidPoison
    : LiquidData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | healthLoss |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnLiquidReception(`LiquidReceiver` liquidReceiver, `Single` dilution, `LiquidContainer` liquidContainer) |  | 


## `LiquidReceiver`

```csharp
public class ThunderRoad.LiquidReceiver
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | colliderReceiver |  | 
| `CollisionHandler` | collisionHandler |  | 
| `String` | drinkEffectId |  | 
| `EffectInstance` | effectInstance |  | 
| `Single` | effectRate |  | 
| `Boolean` | isReceiving |  | 
| `Single` | lastEffectTime |  | 
| `Single` | lastLiquidReceivedTime |  | 
| `LiquidContainer` | liquidContainer |  | 
| `Single` | maxAngle |  | 
| `Vector3` | orgLocalPosition |  | 
| `Quaternion` | orgLocalRotation |  | 
| `Transform` | orgTransform |  | 
| `Single` | stopDelay |  | 


Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `ReceptionEvent` | OnReceptionEvent |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<ValueDropdownItem<String>>` | GetAllEffectID() |  | 
| `void` | OnCreatureDespawn(`EventTime` eventTime) |  | 
| `void` | OnLiquidReceived(`LiquidContainer` liquidContainer) |  | 
| `void` | OnRagdollStateChange(`State` previousState, `State` newState, `PhysicStateChange` physicStateChange, `EventTime` eventTime) |  | 


## `LoadingCamera`

```csharp
public class ThunderRoad.LoadingCamera
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Transform` | canvasRoot |  | 
| `Canvas` | errorCanvas |  | 
| `Text` | errorText |  | 
| `Canvas` | loadingCanvas |  | 
| `Text` | percentage |  | 
| `Single` | rotateThresholdAngle |  | 
| `State` | state |  | 
| `Single` | tipSpeed |  | 
| `Text` | tipsText |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `IEnumerator` | Loading() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioListener` | audioListener |  | 
| `Camera` | cam |  | 
| `UniversalAdditionalCameraData` | cameraData |  | 
| `LoadingCamera` | local |  | 
| `TrackedPoseDriver` | trackedPoseDriver |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | SetPercentage(`Int32` percentage) |  | 
| `void` | SetState(`State` state, `String` errorString = null) |  | 


## `Locomotion`

```csharp
public class ThunderRoad.Locomotion
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `ForceMode` | airForceMode |  | 
| `Single` | airSpeed |  | 
| `Boolean` | allowJump |  | 
| `Boolean` | allowMove |  | 
| `Boolean` | allowTurn |  | 
| `Single` | angularSpeed |  | 
| `Single` | backwardAngle |  | 
| `Single` | backwardspeedMultiplier |  | 
| `CapsuleCollider` | capsuleCollider |  | 
| `PhysicMaterial` | colliderFlyMaterial |  | 
| `PhysicMaterial` | colliderGroundMaterial |  | 
| `Single` | colliderGrowDuration |  | 
| `Single` | colliderHeight |  | 
| `Single` | colliderRadius |  | 
| `Single` | colliderShrinkMinRadius |  | 
| `Single` | crouchHeightRatio |  | 
| `Single` | crouchSpeedRatio |  | 
| `Single` | flyDrag |  | 
| `Single` | forwardAngle |  | 
| `Single` | groundAngle |  | 
| `Single` | groundDetectionDistance |  | 
| `Single` | groundDrag |  | 
| `RaycastHit` | groundHit |  | 
| `Single` | horizontalSpeed |  | 
| `Boolean` | initialized |  | 
| `Boolean` | isGrounded |  | 
| `Boolean` | isJumping |  | 
| `Boolean` | jumpCharging |  | 
| `Single` | jumpChargingTime |  | 
| `Single` | jumpClimbHorizontalMultiplier |  | 
| `Single` | jumpClimbVerticalMaxVelocityRatio |  | 
| `Single` | jumpClimbVerticalMultiplier |  | 
| `Vector3` | jumpForce |  | 
| `Single` | jumpGroundForce |  | 
| `Single` | jumpMaxDuration |  | 
| `Single` | jumpTime |  | 
| `Vector3` | moveDirection |  | 
| `AnimationCurve` | moveForceMultiplierByAngleCurve |  | 
| `List<PhysicModifier>` | physicModifiers |  | 
| `Player` | player |  | 
| `Vector3` | prevPosition |  | 
| `Quaternion` | prevRotation |  | 
| `Vector3` | prevVelocity |  | 
| `Rigidbody` | rb |  | 
| `Single` | runAngle |  | 
| `Boolean` | runEnabled |  | 
| `Single` | runSpeedMultiplier |  | 
| `Single` | snapTurnDelay |  | 
| `Single` | speed |  | 
| `Single` | speedMultiplier |  | 
| `Coroutine` | stopShrinkColliderCoroutine |  | 
| `Single` | strafeSpeedMultiplier |  | 
| `Boolean` | testMove |  | 
| `Single` | turnSmoothDirection |  | 
| `Single` | turnSmoothSnapDirection |  | 
| `Single` | turnSnapDirection |  | 
| `Single` | turnSpeed |  | 
| `Vector3` | velocity |  | 
| `ForceMode` | verticalForceMode |  | 
| `Single` | verticalSpeed |  | 


Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `FlyEvent` | OnFlyEvent |  | 
| `GroundEvent` | OnGroundEvent |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | ClearPhysicModifiers() |  | 
| `void` | FixedUpdate() |  | 
| `void` | Init(`CreatureData` creatureData = null) |  | 
| `void` | Jump(`Boolean` active) |  | 
| `void` | Move(`Vector3` direction) |  | 
| `void` | MoveStop() |  | 
| `void` | MoveWeighted(`Vector3` direction, `Transform` bodyTransform, `Single` heightRatio, `Single` runSpeedRatio = 0, `Single` acceleration = 0) |  | 
| `void` | OnFly() |  | 
| `void` | OnGround(`Vector3` groundPoint, `Vector3` velocity, `Collider` groundCollider) |  | 
| `void` | RefreshPhysicModifiers() |  | 
| `void` | RemovePhysicModifier(`Object` handler) |  | 
| `void` | SetCapsuleCollider(`Single` height) |  | 
| `void` | SetPhysicModifier(`Object` handler, `Int32` priority, `Single` gravityRatio = 1, `Single` massRatio = 1) |  | 
| `Boolean` | SphereCastGround(`Single` castLenght, `RaycastHit&` raycastHit, `Single&` groundDistance) |  | 
| `void` | StartShrinkCollider() |  | 
| `void` | StopShrinkCollider() |  | 
| `IEnumerator` | StopShrinkColliderCoroutine() |  | 
| `void` | Turn(`Single` speed, `TurnMode` turnMode) |  | 
| `void` | Update() |  | 


## `LootTable`

```csharp
public class ThunderRoad.LootTable
    : CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Drop>` | drops |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CalculateWeight() |  | 
| `CatalogData` | Clone() |  | 
| `Int32` | GetCurrentVersion() |  | 
| `void` | OnCatalogRefresh() |  | 
| `ItemData` | Pick(`Int32` pickCount = 0) |  | 


## `Mana`

```csharp
public class ThunderRoad.Mana
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `SpellCaster` | casterLeft |  | 
| `SpellCaster` | casterRight |  | 
| `Single` | chargeSpeedMultiplier |  | 
| `Creature` | creature |  | 
| `Single` | currentFocus |  | 
| `Single` | currentMana |  | 
| `Single` | focusRegen |  | 
| `Boolean` | initialized |  | 
| `Single` | manaRegen |  | 
| `Single` | manaRegenMultiplier |  | 
| `Single` | manaWaste |  | 
| `Single` | maxFocus |  | 
| `Single` | maxMana |  | 
| `Boolean` | mergeActive |  | 
| `Boolean` | mergeCastLoaded |  | 
| `Boolean` | mergeCompleted |  | 
| `SpellMergeData` | mergeData |  | 
| `Single` | mergeHandsDistance |  | 
| `SpellMergeData` | mergeInstance |  | 
| `Transform` | mergePoint |  | 
| `AudioClip` | noManaSound |  | 
| `Collider[]` | overlapColliders |  | 
| `Int32` | overlapCount |  | 
| `Single` | overlapLastTime |  | 
| `LayerMask` | overlapMask |  | 
| `Single` | overlapMinDelay |  | 
| `Single` | overlapRadius |  | 
| `List<SpellPowerData>` | spellPowerInstances |  | 
| `List<SpellData>` | spells |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddSpell(`SpellData` spellData, `Level` level) |  | 
| `Boolean` | CanConsumeFocus(`Single` focusToConsume) |  | 
| `Boolean` | CanConsumeMana(`Single` manaToConsume) |  | 
| `void` | CastOverlapSphere() |  | 
| `void` | ClearSpells() |  | 
| `Boolean` | ConsumeFocus(`Single` focusToConsume) |  | 
| `Boolean` | ConsumeMana(`Single` manaToConsume) |  | 
| `SpellCaster` | GetCaster(`Side` side) |  | 
| `Single` | GetHandsIntensity() |  | 
| `SpellPowerSlowTime` | GetPowerSlowTime() |  | 
| `void` | Init(`Creature` creature) |  | 
| `void` | Load() |  | 
| `void` | OnDisable() |  | 
| `void` | OnHandGrabChangeEvent() |  | 
| `void` | OnSpellChange() |  | 
| `void` | RemoveSpell(`String` spellId = null) |  | 
| `void` | UsePower() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | infiniteFocus |  | 
| `Boolean` | infiniteMana |  | 


## `MaterialData`

```csharp
public class ThunderRoad.MaterialData
    : CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Collision>` | collisions |  | 
| `Collision` | defaultCollision |  | 
| `List<EffectBundle>` | defaultEffects |  | 
| `List<Color>` | idMapColors |  | 
| `Int32` | physicMaterialHash |  | 
| `String` | xpReference |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collision` | GetCollision(`MaterialData` materialData) |  | 
| `Collision` | GetCollision(`Int32` physicMaterialHash) |  | 
| `Int32` | GetCurrentVersion() |  | 
| `void` | OnCatalogRefresh() |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `MaterialData` | GetMaterial(`Collider` collider) |  | 
| `MaterialData` | GetMaterial(`Color` idMapColor) |  | 
| `Boolean` | TryGetMaterials(`Int32` sourcePhysicMaterialHash, `Int32` targetPhysicMaterialHash, `MaterialData&` sourceMaterial, `MaterialData&` targetMaterial) |  | 


## `Menu`

```csharp
public class ThunderRoad.Menu
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<CustomReference>` | customReferences |  | 
| `Transform` | page1 |  | 
| `Transform` | page2 |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Transform` | GetCustomReference(`String` name) |  | 


## `MenuBook`

```csharp
public class ThunderRoad.MenuBook
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `PBook` | book |  | 
| `Single` | closeDelay |  | 
| `Transform` | contentPage1 |  | 
| `Transform` | contentPage2 |  | 
| `Vector3` | handPosition |  | 
| `Coroutine` | hideCoroutine |  | 
| `Single` | lerpSpeed |  | 
| `GameObject` | navBar |  | 
| `Toggle` | navBarToggle |  | 
| `Boolean` | showNavbar |  | 
| `Vector3` | spawnPosition |  | 
| `GameObject` | templateBook |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3` | GetPlayerHandPoint() |  | 
| `Vector3` | GetPlayerSpawnPoint() |  | 
| `IEnumerator` | HideBook() |  | 
| `IEnumerator` | InitCoroutine() |  | 
| `void` | OnBookOpened() |  | 
| `void` | OnBookWillClose() |  | 
| `void` | OnNavButtonValueChanged(`Toggle` toggle, `MenuData` menuData) |  | 
| `void` | RefreshUIObjects() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Texture>` | addressableTextures |  | 
| `Side` | handSide |  | 
| `Boolean` | isShownToPlayer |  | 
| `MenuBook` | local |  | 
| `List<Menu>` | menus |  | 
| `MenuData` | selectedMenuData |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Close() |  | 
| `IEnumerator` | GeneratePages() |  | 
| `void` | Open() |  | 
| `void` | RefreshNavBar() |  | 
| `void` | ReturnToMaster() |  | 
| `void` | SetPage(`String` menuId) |  | 
| `void` | ShowToPlayer(`Boolean` active, `Boolean` navbar = True) |  | 


## `MenuData`

```csharp
public class ThunderRoad.MenuData
    : CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | iconAddress |  | 
| `IResourceLocation` | iconLocation |  | 
| `Boolean` | isDefault |  | 
| `MenuModule` | module |  | 
| `Single` | order |  | 
| `Transform` | page1 |  | 
| `Transform` | page2 |  | 
| `String` | prefabAddress |  | 
| `IResourceLocation` | prefabLocation |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | GetCurrentVersion() |  | 
| `IEnumerator` | OnCatalogRefreshCoroutine() |  | 


## `MenuModule`

```csharp
public class ThunderRoad.MenuModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `MenuData` | menuData |  | 
| `Boolean` | shown |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | GetState() |  | 
| `void` | Init(`MenuData` menuData, `Menu` menu) |  | 
| `void` | OnShow(`Boolean` show) |  | 


## `MenuModuleDebug`

```csharp
public class ThunderRoad.MenuModuleDebug
    : MenuModule

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | GetState() |  | 


## `MenuModuleLocked`

```csharp
public class ThunderRoad.MenuModuleLocked
    : MenuModule

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | GetState() |  | 


## `MenuModuleOptions`

```csharp
public class ThunderRoad.MenuModuleOptions
    : MenuModule

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | GetState() |  | 


## `MenuModuleScores`

```csharp
public class ThunderRoad.MenuModuleScores
    : MenuModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Button` | historyDetailCloseButton |  | 
| `GameObject` | historyDetailPage |  | 
| `GameObject` | historyDetailPrefab |  | 
| `GameObject` | historyLinePrefab |  | 
| `List<HistoryLine>` | historyLines |  | 
| `GameObject` | historyPage |  | 
| `GameObject` | retryButtons |  | 
| `GameObject` | returnHomeButtons |  | 
| `List<UITextScores>` | scoreFields |  | 
| `HistoryEvent` | selectedhistoryEvent |  | 
| `GameObject` | titleDeath |  | 
| `GameObject` | titleDefault |  | 
| `GameObject` | titleFailure |  | 
| `GameObject` | titleSuccess |  | 
| `GameObject` | wave |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | GetState() |  | 
| `void` | Init(`MenuData` menuData, `Menu` menu) |  | 
| `void` | OnHistoryCloseClick() |  | 
| `void` | OnShow(`Boolean` show) |  | 
| `void` | RefreshPage() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `MenuModuleScores` | current |  | 


## `MeshPart`

```csharp
public class ThunderRoad.MeshPart
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `PhysicMaterial` | defaultPhysicMaterial |  | 
| `Int32` | defaultPhysicMaterialHash |  | 
| `Texture2D` | idMap |  | 
| `ManikinPart` | manikinPart |  | 
| `SkinnedMeshRenderer` | skinnedMeshRenderer |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | Raycast(`Vector3` colliderPosition, `Vector3` direction, `MeshRaycastHit&` meshRaycastHit, `SkinnedMeshRenderer` splitRenderer = null) |  | 


## `MeshRaycastHit`

```csharp
public struct ThunderRoad.MeshRaycastHit

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | distance |  | 
| `Vector3` | faceNormal |  | 
| `Int32` | physicMaterialHash |  | 
| `Vector3` | point |  | 
| `Vector2` | textureCoord |  | 
| `Int32` | triangleIndex |  | 


## `Mirror`

```csharp
public class ThunderRoad.Mirror
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Color` | backgroundColor |  | 
| `LayerMask` | cullingMask |  | 
| `Single` | Intensity |  | 
| `MeshRenderer[]` | meshToHide |  | 
| `MeshRenderer` | mirrorMesh |  | 
| `Single` | quality |  | 
| `ReflectionDirection` | reflectionDirection |  | 
| `Boolean` | reflectionWithoutGI |  | 
| `Collider` | workingArea |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ExecuteBeforeCameraRender(`ScriptableRenderContext` context, `Camera` camera) |  | 
| `void` | OnDrawGizmosSelected() |  | 
| `void` | Refresh() |  | 
| `void` | RenderCam(`ScriptableRenderContext` context, `Camera` camera) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Mirror` | local |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DrawGizmoArrow(`Vector3` pos, `Vector3` direction, `Color` color, `Single` arrowHeadLength = 0.25, `Single` arrowHeadAngle = 20) |  | 


## `ModData`

```csharp
public class ThunderRoad.ModData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | Author |  | 
| `String` | Description |  | 
| `String` | folderName |  | 
| `String` | GameVersion |  | 
| `String` | ModVersion |  | 
| `String` | Name |  | 


## `Morphology`

```csharp
public class ThunderRoad.Morphology

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | armsHeight |  | 
| `Single` | armsLength |  | 
| `Single` | armsSpacing |  | 
| `Single` | armsToEyesHeight |  | 
| `Single` | chestHeight |  | 
| `Single` | eyesForward |  | 
| `Single` | eyesHeight |  | 
| `Single` | footHeight |  | 
| `Single` | headForward |  | 
| `Single` | headHeight |  | 
| `Single` | height |  | 
| `Single` | hipsHeight |  | 
| `Single` | legsLength |  | 
| `Single` | legsSpacing |  | 
| `Single` | lowerLegsHeight |  | 
| `Single` | spineHeight |  | 
| `Single` | upperLegsHeight |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Morphology` | Clone() |  | 
| `void` | EstimateProportion() |  | 
| `Single` | GetArmCenterToFingerTipLenght() |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | GetEyesHeight(`Single` height) |  | 
| `Single` | GetHeight(`Single` eyesHeight) |  | 


## `MultiImageButton`

```csharp
public class ThunderRoad.MultiImageButton
    : Button, IMoveHandler, IEventSystemHandler, IPointerDownHandler, IPointerUpHandler, IPointerEnterHandler, IPointerExitHandler, ISelectHandler, IDeselectHandler, IPointerClickHandler, ISubmitHandler

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `TargetGraphicPropagation` | targetGraphicPropagation |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Graphic[]` | Graphics |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DoStateTransition(`SelectionState` state, `Boolean` instant) |  | 


## `Music`

```csharp
public class ThunderRoad.Music
    : CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | fadeInDuration |  | 
| `List<String>` | groupsToLoad |  | 
| `List<MusicGroup>` | loadedMusicGroup |  | 
| `List<MusicTransition>` | transitions |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<ValueDropdownItem<String>>` | GetAllMusicGroupID() |  | 
| `void` | LoadMusicGroups() |  | 
| `void` | OnCatalogRefresh() |  | 
| `IEnumerator` | OnCatalogRefreshCoroutine() |  | 


## `MusicGroup`

```csharp
public class ThunderRoad.MusicGroup
    : CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<MusicSegment>` | loadedMusicSegments |  | 
| `String` | musicGroupName |  | 
| `List<String>` | musicSegments |  | 
| `Boolean` | playInOrder |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<ValueDropdownItem<String>>` | GetAllMusicSegmentID() |  | 
| `IEnumerator` | LoadAll() |  | 
| `IEnumerator` | OnCatalogRefreshCoroutine() |  | 


## `MusicManager`

```csharp
public class ThunderRoad.MusicManager
    : MonoBehaviour

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Load(`String` aMusicName) |  | 
| `void` | Test(`String` musicType) |  | 
| `void` | TestChase() |  | 
| `void` | TestDefault() |  | 
| `void` | TestFight() |  | 
| `void` | TestTension() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioClip[]` | audioClipArray |  | 
| `AudioSource[]` | audioSourceArray |  | 
| `MusicManager` | local |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ChangeMusicType(`String` musicType) |  | 
| `IEnumerator` | LoadMusics(`String` aMusicName) |  | 
| `void` | OnPlayerExposureChangeEvent(`Exposure` oldExposure, `Exposure` newExposure) |  | 


## `MusicSegment`

```csharp
public class ThunderRoad.MusicSegment
    : CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioClip` | audioClip |  | 
| `Int32` | beatsPerBar |  | 
| `Int32` | BPM |  | 
| `String` | musicAddress |  | 
| `IResourceLocation` | musicLocation |  | 
| `String` | name |  | 
| `Single` | volume |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `IEnumerator` | LoadSegment() |  | 
| `IEnumerator` | OnCatalogRefreshCoroutine() |  | 


## `NoiseManager`

```csharp
public class ThunderRoad.NoiseManager
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | noiseCount |  | 
| `Noise[]` | noises |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | GetFreeNoiseIndex() |  | 
| `void` | OnDisable() |  | 
| `void` | OnEnable() |  | 
| `void` | Reset() |  | 
| `void` | SlowUpdate() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `NoiseManager` | instance |  | 
| `Boolean` | isActive |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Noise` | AddLoopNoise(`AudioSource` audioSource, `Creature` sourceCreature = null) |  | 
| `Noise` | AddNoise(`Vector3` position, `Single` volume, `Creature` sourceCreature = null) |  | 
| `void` | RemoveLoopNoise(`AudioSource` audioSource) |  | 
| `Boolean` | TryGetLouderNoise(`Creature` fromCreature, `Single` range, `Noise&` noise, `Single&` louderNoise) |  | 


## `ObjectSlider`

```csharp
public class ThunderRoad.ObjectSlider
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | audioReachMaxVelocity |  | 
| `Single` | audioReachMinVelocity |  | 
| `CollisionHandler` | collisionHandler |  | 
| `Single` | currentPosition |  | 
| `Vector2` | driveDamper |  | 
| `Boolean` | driveEnabled |  | 
| `Vector2` | driveMaxForce |  | 
| `Single` | drivePositionOnStart |  | 
| `Vector2` | driveSpring |  | 
| `Coroutine` | dynamicDriveCoroutine |  | 
| `AnimationCurve` | dynamicDriveCurve |  | 
| `Single` | dynamicDriveCurveDuration |  | 
| `Boolean` | dynamicDriveEnabled |  | 
| `Single` | dynamicDriveSpeed |  | 
| `FxModuleAudio` | effectAudioReachEnd |  | 
| `FxModuleAudio` | effectAudioReachStart |  | 
| `Boolean` | haveNavMeshObstacle |  | 
| `Boolean` | initialized |  | 
| `ConfigurableJoint` | joint |  | 
| `JointDrive` | jointDrive |  | 
| `Single` | maxheight |  | 
| `NavMeshObstacle` | navMeshObstacle |  | 
| `Single` | navMeshObstacleMaxHeight |  | 
| `Single` | positionOnStart |  | 
| `Single` | reachOffset |  | 
| `Transform` | startTransform |  | 
| `State` | state |  | 
| `UnityEvent` | targetReachEvent |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | Close() |  | 
| `Single` | GetDrivePosition() |  | 
| `void` | HoldDrive() |  | 
| `void` | OnDrawGizmos() |  | 
| `void` | OnEnable() |  | 
| `void` | Open() |  | 
| `void` | SetDrive(`Single` linearPosition) |  | 
| `void` | SetJointTargetPosition(`Single` linearPosition) |  | 
| `void` | SetPosition(`Single` linearPosition) |  | 
| `void` | Start() |  | 
| `void` | StopDrive() |  | 
| `void` | Update() |  | 


## `ObjectViewer`

```csharp
public class ThunderRoad.ObjectViewer
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | active |  | 
| `Camera` | cam |  | 
| `Light` | camLight |  | 
| `Int32` | orgLayer |  | 
| `RenderTexture` | renderTexture |  | 
| `Transform` | rootCam |  | 
| `Vector3` | rotation |  | 
| `Item` | targetObject |  | 
| `Renderer` | targetRenderer |  | 
| `String` | tempLayer |  | 
| `List<VisibleObject>` | visibleObjects |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AlignCamera(`Transform` target) |  | 
| `void` | Awake() |  | 
| `void` | StartRender(`Item` targetObject, `RenderTexture` renderTexture) |  | 
| `void` | StopRenderer() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `ObjectViewer` | local |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | CreateDummyObject(`Item` itemPrefab) |  | 
| `IEnumerator` | CreateIcon(`ItemData` itemData) |  | 


## `Ocean`

```csharp
public class ThunderRoad.Ocean
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `OceanDepthCache` | crestOceanDepthCache |  | 
| `OceanRenderer` | crestOceanRenderer |  | 
| `ShapeFFT` | crestShapeFFT |  | 
| `ShapeGerstner` | crestShapeGerstner |  | 
| `String` | lowQualityPrefabAddress |  | 
| `GameObject` | oceanGameobject |  | 
| `MeshRenderer` | oceanLowQualityMeshRenderer |  | 
| `String` | prefabAddress |  | 
| `Room` | room |  | 
| `Boolean` | showWhenInRoomOnly |  | 
| `Boolean` | spawning |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | SetActive(`Boolean` active) |  | 
| `void` | Spawn() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Ocean>` | all |  | 
| `Ocean` | current |  | 
| `Quality` | quality |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | SetQuality(`Quality` quality) |  | 


## `OculusMRC`

```csharp
public class ThunderRoad.OculusMRC
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `LayerMask` | hiddenLayers |  | 
| `LayerMask` | visibleLayers |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `OculusMRC` | instance |  | 
| `State` | state |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | SetState(`State` state) |  | 


## `Options`

```csharp
public class ThunderRoad.Options

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | allowStickJump |  | 
| `Boolean` | allowStickPressJump |  | 
| `Single` | ambientVolume |  | 
| `Single` | armMaxLengthMultiplier |  | 
| `Boolean` | bloodEffects |  | 
| `Boolean` | bloomEnabled |  | 
| `Single` | bloomIntensity |  | 
| `Single` | bloomThreshold |  | 
| `Boolean` | cleanVisibleDeads |  | 
| `Boolean` | comfortVignette |  | 
| `Single` | contrast |  | 
| `List<Controller>` | controllers |  | 
| `Boolean` | crouchOnJump |  | 
| `Boolean` | dismembermentEnabled |  | 
| `Single` | effectVolume |  | 
| `Boolean` | enableCharacterReveal |  | 
| `Boolean` | enableExternalView |  | 
| `Boolean` | enableItemReveal |  | 
| `Boolean` | eyeAdaptation |  | 
| `Int32` | foveationLevel |  | 
| `Boolean` | handleForceXYZ |  | 
| `Int32` | handlePositionDamperMultiplier |  | 
| `Int32` | handlePositionSpringMultiplier |  | 
| `Int32` | handleRotationDamperMultiplier |  | 
| `Int32` | handleRotationSpringMultiplier |  | 
| `Boolean` | healthVignette |  | 
| `String` | language |  | 
| `Side` | locomotionController |  | 
| `LocomotionDirection` | locomotionDirection |  | 
| `Int32` | maleRatio |  | 
| `Single` | masterVolume |  | 
| `Int32` | maxDeadCount |  | 
| `Int32` | maxDecals |  | 
| `Int32` | maxDropCount |  | 
| `Int32` | monitorHeight |  | 
| `Int32` | monitorWidth |  | 
| `Int32` | msaa |  | 
| `Single` | musicVolume |  | 
| `Quality` | oceanQuality |  | 
| `State` | oculusMrcState |  | 
| `Boolean` | outline |  | 
| `PhysicTimeStep` | physicTimeStep |  | 
| `RuntimePlatform` | platform |  | 
| `Boolean` | pointerRay |  | 
| `Single` | postExposure |  | 
| `Boolean` | postProcessing |  | 
| `QualityPreset` | qualityPreset |  | 
| `Single` | renderScale |  | 
| `Int32` | screenshotFov |  | 
| `Int32` | screenshotHeight |  | 
| `Int32` | screenshotWidth |  | 
| `Boolean` | setResolutionOnStart |  | 
| `Single` | shadowDistance |  | 
| `Single` | sharpen |  | 
| `Boolean` | showDistantHighlighter |  | 
| `Boolean` | showHudHighlighter |  | 
| `Boolean` | showTouchHighlighter |  | 
| `CrouchMode` | stickCrouchMode |  | 
| `StuckBehaviour` | stuckBehaviour |  | 
| `Int32` | textureLimit |  | 
| `TonemappingMode` | toneMapping |  | 
| `TurnMode` | turnMode |  | 
| `Single` | turnSpeed |  | 
| `Side` | twoHandedDominantHand |  | 
| `TwoHandedMode` | twoHandedMode |  | 
| `Side` | uiPointerHand |  | 
| `Single` | uiVolume |  | 
| `Int32` | version |  | 
| `Single` | vibrance |  | 
| `Single` | voiceVolume |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Apply() |  | 
| `Controller` | GetController() |  | 
| `void` | OnLevelLoading() |  | 
| `void` | ResetControllers() |  | 
| `void` | ResetPostProcess() |  | 
| `void` | SetHoldGripToGrab(`Boolean` active) |  | 
| `void` | SetQualityPreset() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | newVersion |  | 


## `PageViewer`

```csharp
public class ThunderRoad.PageViewer
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Button` | buttonNext |  | 
| `Button` | buttonPrevious |  | 
| `Int32` | currentPage |  | 
| `Image` | image |  | 
| `String` | pageGroupId |  | 
| `Text` | text |  | 
| `Text` | title |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `List<ValueDropdownItem<String>>` | GetAllPageGroupsId() |  | 
| `void` | Next() |  | 
| `void` | Previous() |  | 
| `void` | Refresh() |  | 


## `ParryTarget`

```csharp
public class ThunderRoad.ParryTarget
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Item` | item |  | 
| `Single` | length |  | 
| `Creature` | owner |  | 
| `Collider` | testCollider |  | 
| `Side` | testSide |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `Vector3` | GetLineEnd() |  | 
| `Vector3` | GetLineStart() |  | 
| `ParryInfo` | GetParryPositionAndRotation(`Collider` defenseCollider) |  | 
| `void` | OnDisable() |  | 
| `void` | OnGrab(`Handle` handle, `RagdollHand` ragdollHand) |  | 
| `void` | OnRelease(`Handle` handle, `RagdollHand` ragdollHand, `Boolean` throwing) |  | 
| `void` | OnSnap(`Holder` handle) |  | 
| `void` | OnThrowingEnd() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<ParryTarget>` | list |  | 


## `ParticleCollisionSpawner`

```csharp
public class ThunderRoad.ParticleCollisionSpawner
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | active |  | 
| `List<ParticleCollisionEvent>` | collisionEvents |  | 
| `EffectData` | effectData |  | 
| `EffectParticle` | effectParticle |  | 
| `ParticleSystem` | particle |  | 


## `Platform`

```csharp
public enum ThunderRoad.Platform
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | Windows |  | 
| `1` | Quest2 |  | 
| `2` | PSVR |  | 


## `PlatformStore`

```csharp
public class ThunderRoad.PlatformStore

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | GetUserName() |  | 
| `void` | Unload() |  | 
| `void` | Update() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Callback` | callback |  | 


## `PlatformStoreHtc`

```csharp
public class ThunderRoad.PlatformStoreHtc
    : PlatformStore

```

Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Coroutine` | checkCoroutine |  | 


## `PlatformStoreOculus`

```csharp
public class ThunderRoad.PlatformStoreOculus
    : PlatformStore

```

## `PlatformStoreSteam`

```csharp
public class ThunderRoad.PlatformStoreSteam
    : PlatformStore

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | GetUserName() |  | 
| `Boolean` | Init(`UInt32` steamAppID, `String&` errorMessage) |  | 
| `void` | Unload() |  | 
| `void` | Update() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | initialized |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | GetAuthSessionTicket() |  | 
| `void` | SteamInfo() |  | 


## `PlatformStoreSynthesis`

```csharp
public class ThunderRoad.PlatformStoreSynthesis
    : PlatformStore

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `IPEndPoint` | localpt |  | 
| `UdpClient` | udpDiscoveryListener |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | Filehash(`String` fileName) |  | 
| `void` | StartUdpDiscovery() |  | 
| `void` | UdpDiscoveryDataReceived(`IAsyncResult` ar) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<String>` | IPAddresses |  | 
| `ArcadeInterface` | svrInterface |  | 
| `String` | synthesisGameId |  | 
| `Int32` | udpPort |  | 
| `Boolean` | winServerForAndroid |  | 


## `Player`

```csharp
public class ThunderRoad.Player
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | copyLocomotionParameterFromBody |  | 
| `Creature` | creature |  | 
| `Single` | crouchHeightOffset |  | 
| `Boolean` | crouching |  | 
| `Single` | crouchLandingMaxDuration |  | 
| `Single` | crouchLandingMaxSpeed |  | 
| `Single` | crouchLandingMinDuration |  | 
| `Single` | crouchLandingMinSpeed |  | 
| `Single` | crouchMinHeight |  | 
| `Single` | crouchSpeedGround |  | 
| `Single` | crouchSpeedJump |  | 
| `PlayerFoot` | footLeft |  | 
| `PlayerFoot` | footRight |  | 
| `PlayerHand` | handLeft |  | 
| `PlayerHand` | handRight |  | 
| `PlayerHead` | head |  | 
| `Boolean` | isLocal |  | 
| `Single` | kickLocomotionMaxSpeed |  | 
| `AnimationCurve` | landStandingLightCurve |  | 
| `AnimationCurve` | landStandingStrongCurve |  | 
| `Vector3` | lastPresencePosition |  | 
| `Quaternion` | lastPresenceRotation |  | 
| `Boolean` | lastPresenceSaved |  | 
| `Locomotion` | locomotion |  | 
| `Transform` | offsetTransform |  | 
| `Single` | orgAngularDrag |  | 
| `Single` | orgDrag |  | 
| `Single` | orgMass |  | 
| `Quaternion` | prevRotation |  | 
| `Boolean` | showMorphology |  | 
| `PlayerWaist` | waist |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | Calibrate(`Creature` creature, `Boolean` moveBody = True) |  | 
| `void` | CopyLocomotionValuesFrom(`Locomotion` source) |  | 
| `void` | FixedUpdate() |  | 
| `PlayerFoot` | GetFoot(`Side` side) |  | 
| `PlayerHand` | GetHand(`Side` side) |  | 
| `Single` | GetHeightOffset() |  | 
| `Vector3` | GetShoulderCenter() |  | 
| `void` | OnDrawGizmos() |  | 
| `void` | OnLocomotionFlyEvent() |  | 
| `void` | OnLocomotionGroundEvent(`Vector3` groundPoint, `Vector3` velocity, `Collider` groundCollider) |  | 
| `void` | OnVRPresence(`Boolean` active) |  | 
| `void` | ReleaseCreature() |  | 
| `void` | SetCreature(`Creature` targetCreature, `Boolean` physicBody = False) |  | 
| `void` | SetHeightOffset(`Single` value) |  | 
| `void` | SetVisibilityDistance(`Single` sightDistance) |  | 
| `void` | Teleport(`Transform` targetTransform, `Boolean` keepVelocity = False) |  | 
| `void` | Teleport(`Vector3` position, `Quaternion` rotation, `Boolean` keepVelocity = False) |  | 
| `void` | Update() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `PlayerCharacterData` | characterData |  | 
| `Boolean` | crouchOnJump |  | 
| `Creature` | currentCreature |  | 
| `Boolean` | fallDamage |  | 
| `Single` | heightOffset |  | 
| `Boolean` | invincibility |  | 
| `Player` | local |  | 
| `Boolean` | selfCollision |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Morphology` | GetMorphology(`Transform` playArea, `Vector3` eyesPosition, `Vector3` handLPos1, `Vector3` handLPos2, `Vector3` handLPos3, `Vector3` handLPos4, `Vector3` handRPos1, `Vector3` handRPos2, `Vector3` handRPos3, `Vector3` handRPos4) |  | 
| `Player` | Spawn(`Transform` targetTransform) |  | 
| `Player` | Spawn(`Vector3` position, `Quaternion` rotation) |  | 


Static Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `SpawnEvent` | onSpawn |  | 


## `PlayerCharacterData`

```csharp
public class ThunderRoad.PlayerCharacterData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | calibrated |  | 
| `String` | creatureId |  | 
| `Color` | eyesIrisColor |  | 
| `Color` | eyesScleraColor |  | 
| `GameMode` | gameMode |  | 
| `String` | gameModeId |  | 
| `Color` | hairColor |  | 
| `Color` | hairSecondaryColor |  | 
| `Color` | hairSpecularColor |  | 
| `Single` | height |  | 
| `List<Content>` | homeInventory |  | 
| `String` | ID |  | 
| `List<Content>` | inventory |  | 
| `Vector3` | leftFootTrackerLocalPosition |  | 
| `Quaternion` | leftFootTrackerLocalRotation |  | 
| `Vector3` | rightFootTrackerLocalPosition |  | 
| `Quaternion` | rightFootTrackerLocalRotation |  | 
| `List<SavedCreature>` | savedCreatures |  | 
| `Color` | skinColor |  | 
| `Int32` | tipIndex |  | 
| `Tutorial` | tutorial |  | 
| `Int32` | version |  | 
| `Vector3` | waistTrackerBoneLocalPosition |  | 
| `Quaternion` | waistTrackerBoneLocalRotation |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | Check() |  | 
| `List<Content>` | CloneInventory() |  | 
| `String` | GetCreatureID() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Tutorial` | forceTutorial |  | 
| `Int32` | newVersion |  | 


## `PlayerControl`

```csharp
public class ThunderRoad.PlayerControl
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | axisExternalViewHeightDeadZone |  | 
| `Single` | axisHeightDeadZone |  | 
| `Single` | axisMoveDeadZone |  | 
| `Single` | axisTurnDeadZone |  | 
| `ComboButton` | comboButton |  | 
| `Single` | currentRunSwingRatio |  | 
| `XRLoader` | currentXRLoader |  | 
| `InputDevice` | headDevice |  | 
| `Boolean` | jumpEnabled |  | 
| `Boolean` | jumpPressed |  | 
| `Boolean` | jumpStickUp |  | 
| `Boolean` | kickEnabled |  | 
| `LayerMask` | kickRayLayer |  | 
| `Single` | kickRayLenght |  | 
| `Single` | kickRayRadius |  | 
| `Side` | locomotionController |  | 
| `LocomotionDirection` | locomotionDirection |  | 
| `Single` | maxRunSwingSpeed |  | 
| `Single` | minRunSwingSpeed |  | 
| `Single` | minSpellSelectionMagnitude |  | 
| `Boolean` | moveEnabled |  | 
| `Single` | notIndexMinCurl |  | 
| `Single` | runSwingSmoothing |  | 
| `Single` | scrollSpeed |  | 
| `Single` | snapTurnDelay |  | 
| `Single` | snapTurnSpeed |  | 
| `Boolean` | turnEnabled |  | 
| `TurnMode` | turnMode |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AlternateUse(`Side` side, `Single` axis) |  | 
| `void` | Cast(`Side` side, `Single` axis) |  | 
| `void` | ExternalViewHeight(`Single` axis) |  | 
| `Vector3` | GetFootPosition(`Side` side) |  | 
| `Quaternion` | GetFootRotation(`Side` side) |  | 
| `Boolean` | GetFootTracking(`Side` side) |  | 
| `Vector3` | GetFootVelocity(`Side` side) |  | 
| `Vector3[]` | GetHandBonePositions(`Side` side) |  | 
| `Quaternion[]` | GetHandBoneRotations(`Side` side) |  | 
| `Single` | GetHeightAxis(`Single` axisY) |  | 
| `Vector3` | GetMoveDirection(`Side` side, `Vector2` axis) |  | 
| `Single` | GetTurnAxis(`Single` axisX) |  | 
| `Vector3` | GetWaistPosition() |  | 
| `Quaternion` | GetWaistRotation() |  | 
| `Boolean` | GetWaistTracking() |  | 
| `Vector3` | GetWaistVelocity() |  | 
| `XRLoader` | GetXRLoader(`Loader` loader) |  | 
| `Boolean` | Grab(`Side` side) |  | 
| `Boolean` | GrabGrip(`Side` side) |  | 
| `Boolean` | GrabPinch(`Side` side) |  | 
| `void` | Jump(`Boolean` active) |  | 
| `void` | Kick(`Boolean` active) |  | 
| `void` | Move(`Side` side, `Vector2` axis) |  | 
| `void` | MoveActive(`Boolean` active) |  | 
| `void` | Screenshot() |  | 
| `Boolean` | ScrollUI(`Side` side, `Vector2` axis) |  | 
| `void` | ShowDevices() |  | 
| `Boolean` | SpellSelection(`Side` side, `Boolean` active) |  | 
| `Boolean` | TelekinesisAxis(`Side` side, `Vector2` axis) |  | 
| `Boolean` | TelekinesisGrab(`Side` side) |  | 
| `Boolean` | TelekinesisPull(`Side` side, `Single` value, `Boolean` grabReady = True) |  | 
| `Boolean` | TelekinesisRelease(`Side` side) |  | 
| `Boolean` | TelekinesisRepel(`Side` side, `Single` value) |  | 
| `Boolean` | TelekinesisToogleSpin(`Side` side) |  | 
| `void` | ToogleExternalView() |  | 
| `void` | ToogleExternalViewLock() |  | 
| `void` | ToogleMenu(`Boolean` isChainAction) |  | 
| `void` | Turn(`Side` side, `Vector2` axis, `Boolean` leftRightOnly = False) |  | 
| `void` | TurnActive(`Boolean` active) |  | 
| `Boolean` | Ungrab(`Side` side) |  | 
| `Boolean` | UngrabGrip(`Side` side) |  | 
| `Boolean` | UngrabPinch(`Side` side) |  | 
| `void` | Use(`Side` side, `Single` axis) |  | 
| `void` | UsePower() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | chainActionDone |  | 
| `Boolean` | chainButtonPressed |  | 
| `Controller` | controller |  | 
| `ControllerDiagram` | controllerDiagram |  | 
| `Boolean` | externalViewLocked |  | 
| `Hand` | handLeft |  | 
| `Hand` | handRight |  | 
| `InputBase` | input |  | 
| `Boolean` | inputLoaded |  | 
| `Boolean` | leftDirWaitZero |  | 
| `Loader` | loader |  | 
| `PlayerControl` | local |  | 
| `Boolean` | moveActive |  | 
| `OnDeviceConnected` | onDeviceConnected |  | 
| `OnSystemMenu` | onSystemMenu |  | 
| `OnUserPresence` | onUserPresenceChange |  | 
| `OnVRPresence` | onVRPresence |  | 
| `Boolean` | pressToMove |  | 
| `Boolean` | rightDirWaitZero |  | 
| `Boolean` | systemMenuActive |  | 
| `Boolean` | turnActive |  | 
| `Boolean` | uiClickDown |  | 
| `Boolean` | uiClickUp |  | 
| `Boolean` | userPresence |  | 
| `Boolean` | vrEnabled |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Hand` | GetHand(`Side` side) |  | 
| `IEnumerator` | Init() |  | 
| `void` | InvokeSystemMenu(`Boolean` active) |  | 
| `void` | OnDeviceConnectedEvent(`Device` device, `Boolean` connected) |  | 
| `void` | SetFoveationLevel(`Int32` level) |  | 
| `void` | SetInputs(`Boolean` active) |  | 
| `void` | TestFoveationLevel() |  | 


## `PlayerControlTest`

```csharp
public class ThunderRoad.PlayerControlTest
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | enableMove |  | 
| `HapticClip` | hapticClip |  | 
| `Single` | hapticClipAmplitude |  | 
| `Boolean` | hapticLoop |  | 
| `Single` | hapticLoopIntensity |  | 
| `Single` | hapticLoopPeriod |  | 


## `PlayerFoot`

```csharp
public class ThunderRoad.PlayerFoot
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3` | animBonePosition |  | 
| `Quaternion` | animBoneRotation |  | 
| `Coroutine` | autoKickCoroutine |  | 
| `Boolean` | footTracked |  | 
| `Rigidbody` | grip |  | 
| `Boolean` | isAutoKicking |  | 
| `Single` | kickExtendDuration |  | 
| `Single` | kickExtendRatio |  | 
| `Single` | kickFlyHeightRatio |  | 
| `Single` | kickFoldRatio |  | 
| `Single` | kickGroundHeightRatio |  | 
| `Single` | kickMaxHeightRatio |  | 
| `Single` | kickReturnDuration |  | 
| `Single` | kickStayDuration |  | 
| `PlayerLink` | link |  | 
| `MeshRenderer` | marker |  | 
| `Player` | player |  | 
| `Single` | playerMinHeight |  | 
| `Single` | playerMinSpeed |  | 
| `RagdollFoot` | ragdollFoot |  | 
| `Boolean` | resetPosOnUserAbsence |  | 
| `Side` | side |  | 
| `Boolean` | trackController |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | CheckTracking() |  | 
| `PlayerFoot` | GetOtherFoot() |  | 
| `void` | Kick(`Transform` target, `Vector3` targetLocalPos) |  | 
| `void` | OnDeviceConnected(`Device` device, `Boolean` connected) |  | 
| `void` | OnDisable() |  | 
| `void` | OnEnable() |  | 
| `void` | OnPreIKUpdateEvent() |  | 
| `void` | OnUserPresenceChange() |  | 
| `void` | RefreshFootState() |  | 
| `void` | ReleaseCreature() |  | 
| `void` | SetCreature(`RagdollFoot` ragdollFoot) |  | 
| `void` | SetDefaultPosition() |  | 
| `void` | SetFootTracking(`Boolean` active) |  | 
| `void` | Update() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | autoKick |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Kick(`Boolean` active) |  | 


## `PlayerHand`

```csharp
public class ThunderRoad.PlayerHand
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `LayerMask` | collisionUngrabLayerMask |  | 
| `Hand` | controlHand |  | 
| `Vector3` | defaultPosition |  | 
| `Vector3` | defaultRotation |  | 
| `LayerMask` | fingerCollisionLayerMask |  | 
| `Rigidbody` | grip |  | 
| `PlayerLink` | link |  | 
| `MeshRenderer` | noBodyMesh |  | 
| `Player` | player |  | 
| `RagdollHand` | ragdollHand |  | 
| `Boolean` | resetPosOnUserAbsence |  | 
| `Transform` | root |  | 
| `Side` | side |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `PlayerHand` | GetOtherHand() |  | 
| `void` | OnDisable() |  | 
| `void` | OnEnable() |  | 
| `void` | OnGrabEvent(`Side` side, `Handle` handle, `Single` axisPosition, `HandleOrientation` orientation, `EventTime` eventTime) |  | 
| `void` | OnUnGrabEvent(`Side` side, `Handle` handle, `Boolean` throwing, `EventTime` eventTime) |  | 
| `void` | OnUserPresenceChange() |  | 
| `void` | RefreshTracking() |  | 
| `void` | ReleaseCreature() |  | 
| `void` | SetCreature(`RagdollHand` ragdollHand) |  | 
| `void` | SetDefaultPosition() |  | 
| `void` | SetTracking(`Boolean` active) |  | 
| `void` | Update() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `StuckBehaviour` | stuckBehaviour |  | 


## `PlayerHead`

```csharp
public class ThunderRoad.PlayerHead
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Transform` | anchor |  | 
| `AudioListener` | audioListener |  | 
| `Camera` | cam |  | 
| `UniversalAdditionalCameraData` | cameraData |  | 
| `Transform` | highlighterRootLeft |  | 
| `Transform` | highlighterRootRight |  | 
| `PerfectCullingCamera` | perfectCullingCamera |  | 
| `Player` | player |  | 
| `SphereCollider` | sphereCollider |  | 
| `TrackedPoseDriver` | trackedPoseDriver |  | 
| `Boolean` | useTrackedPoseDriver |  | 
| `MeshRenderer` | vignetteMesh |  | 
| `MaterialPropertyBlock` | vignetteMeshMaterialPropertyBlock |  | 
| `Int32` | vignettePropertyIdColor |  | 
| `Int32` | vignettePropertyIdOpacity |  | 
| `Int32` | vignettePropertyIdSize |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | OnDisable() |  | 
| `void` | OnEnable() |  | 
| `void` | OnUserPresenceChange() |  | 
| `void` | RefreshTracking() |  | 
| `void` | RefreshVignette() |  | 
| `void` | SetDefaultPosition() |  | 
| `void` | SetTracking(`Boolean` active) |  | 
| `void` | SetVignette(`Boolean` active) |  | 
| `void` | SetVignetteColor(`Color` color) |  | 
| `void` | SetVignetteOpacity(`Single` opacity) |  | 
| `void` | SetVignetteSize(`Single` size) |  | 


## `PlayerLink`

```csharp
public class ThunderRoad.PlayerLink
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Rigidbody` | attachedRigidbody |  | 
| `ConfigurableJoint` | controllerJoint |  | 
| `Rigidbody` | controllerRigidbody |  | 
| `Boolean` | forcePlayerJoint |  | 
| `Boolean` | gripping |  | 
| `Boolean` | isActive |  | 
| `Boolean` | itemForcePlayerJoint |  | 
| `Player` | player |  | 
| `ConfigurableJoint` | playerJoint |  | 
| `Boolean` | playerJointActive |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Attach(`Rigidbody` rigidbody, `Transform` node, `Boolean` teleport, `Boolean` gripping = False, `Boolean` itemForcePlayerJoint = False) |  | 
| `void` | AttachRagdollPart(`RagdollPart` ragdollPart, `Transform` grip) |  | 
| `void` | Awake() |  | 
| `void` | Detach() |  | 
| `void` | DetachRagdollPart(`RagdollPart` ragdollPart) |  | 
| `void` | FixedUpdate() |  | 
| `void` | OnLocomotionFlyEvent() |  | 
| `void` | OnLocomotionGroundEvent(`Vector3` groundPoint, `Vector3` velocity, `Collider` groundCollider) |  | 
| `void` | RefreshJointConfig() |  | 
| `void` | SetJointConfig(`ConfigurableJoint` joint, `Vector2` positionMultiplier, `Vector2` rotationMultiplier, `Single` maxPositionForce, `Single` maxRotationForce, `Single` limit = 0) |  | 
| `void` | Start() |  | 


## `PlayerSpawner`

```csharp
public class ThunderRoad.PlayerSpawner
    : MonoBehaviour

```

Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<PlayerSpawner>` | all |  | 
| `List<PlayerSpawner>` | allActive |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `PlayerSpawner` | Get() |  | 


## `PlayerTest`

```csharp
public class ThunderRoad.PlayerTest
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Camera` | cam |  | 
| `UniversalAdditionalCameraData` | cameraData |  | 
| `CapsuleCollider` | collider |  | 
| `Single` | jumpForce |  | 
| `Single` | moveSpeed |  | 
| `Rigidbody` | rigidbody |  | 
| `Single` | turnSpeed |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `PlayerTest` | local |  | 


Static Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `SpawnEvent` | onSpawn |  | 


## `PlayerTestHand`

```csharp
public class ThunderRoad.PlayerTestHand
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `InputDevice` | device |  | 
| `FixedJoint` | fixedJoint |  | 
| `Rigidbody` | grabbedRb |  | 
| `Boolean` | gripPressState |  | 
| `Boolean` | orgKinematic |  | 
| `Boolean` | primaryPressState |  | 
| `Rigidbody` | rb |  | 
| `Boolean` | secondaryPressState |  | 
| `XRNode` | xrNode |  | 


## `PlayerWaist`

```csharp
public class ThunderRoad.PlayerWaist
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Creature` | creature |  | 
| `Transform` | ikAnchor |  | 
| `MeshRenderer` | marker |  | 
| `Player` | player |  | 
| `Boolean` | resetPosOnUserAbsence |  | 
| `Boolean` | trackController |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | CheckTracking() |  | 
| `void` | OnDeviceConnected(`Device` device, `Boolean` connected) |  | 
| `void` | OnDisable() |  | 
| `void` | OnEnable() |  | 
| `void` | OnUserPresenceChange() |  | 
| `void` | ReleaseCreature() |  | 
| `void` | SetCreature(`Creature` creature) |  | 
| `void` | SetDefaultPosition() |  | 
| `void` | Start() |  | 
| `void` | Update() |  | 


## `Pointer`

```csharp
public class ThunderRoad.Pointer
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioSource` | audioSource |  | 
| `GameObject` | cursor |  | 
| `Single` | cursorMaxScale |  | 
| `Single` | cursorMinScale |  | 
| `GameObject` | cursorPrefab |  | 
| `Boolean` | isPointingUI |  | 
| `LayerMask` | layerMask |  | 
| `MeshRenderer` | mesh |  | 
| `Color` | meshEmissionColor |  | 
| `Single` | meshEmissionColorChangeSpeed |  | 
| `Color` | meshEmissionCurrentColor |  | 
| `Vector3` | meshLocalPosition |  | 
| `AssetReferenceGameObject` | meshReference |  | 
| `PlayerHand` | playerHand |  | 
| `Vector3` | pointerRayLocalPosition |  | 
| `Transform` | pointerRaySource |  | 
| `Transform` | pointerRayTarget |  | 
| `VisualEffect` | pointerVisualEffectRay |  | 
| `ScrollRect` | scrollRect |  | 
| `GameObject` | target |  | 


Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `PointingEvent` | OnPointingEvent |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | ButtonDown() |  | 
| `Boolean` | ButtonUp() |  | 
| `void` | OnDisable() |  | 
| `void` | OnEnterControl(`GameObject` control) |  | 
| `void` | OnExitControl(`GameObject` control) |  | 
| `void` | StopPointing() |  | 
| `void` | Update() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Side` | activeSide |  | 
| `Boolean` | clickEnabled |  | 
| `Pointer` | left |  | 
| `Single` | raycastDistance |  | 
| `Pointer` | right |  | 
| `Boolean` | showMesh |  | 
| `Boolean` | showRay |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Pointer` | GetActive() |  | 
| `Pointer` | GetPointer(`Side` side) |  | 
| `void` | ShowMesh(`Boolean` active) |  | 


## `PointerEventData`

```csharp
public class ThunderRoad.PointerEventData
    : PointerEventData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | current |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Reset() |  | 


## `PointerInputModule`

```csharp
public class ThunderRoad.PointerInputModule
    : BaseInputModule

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `LayerMask` | layerMask |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | ClearSelection() |  | 
| `void` | Process() |  | 
| `void` | Start() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | active |  | 
| `GameObject` | currentDragging |  | 
| `GameObject` | currentPoint |  | 
| `GameObject` | currentPressed |  | 
| `Pointer` | pointer |  | 
| `PointerEventData` | pointerEvent |  | 


Static Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `PointerInputModule` | local |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | SetUICameraToAllCanvas() |  | 


## `PrefabSpawner`

```csharp
public class ThunderRoad.PrefabSpawner
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | address |  | 
| `Plateform` | plateform |  | 
| `Boolean` | spawnOnStart |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Spawn() |  | 
| `void` | Start() |  | 


## `Preview`

```csharp
public class ThunderRoad.Preview
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture2D` | generatedIcon |  | 
| `Int32` | iconResolution |  | 
| `List<Renderer>` | renderers |  | 
| `Single` | size |  | 
| `Int32` | tempLayer |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnDrawGizmosSelected() |  | 


## `Ragdoll`

```csharp
public class ThunderRoad.Ragdoll
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | allowSelfDamage |  | 
| `Transform` | animatorRig |  | 
| `List<Bone>` | bones |  | 
| `Boolean` | charJointBreakEnabled |  | 
| `Single` | collisionEffectMinDelay |  | 
| `Single` | collisionMinVelocity |  | 
| `Creature` | creature |  | 
| `Single` | damperPositionForce |  | 
| `Single` | damperRotationForce |  | 
| `Single` | destabilizedDamperRotationMultiplier |  | 
| `Single` | destabilizedGroundSpringRotationMultiplier |  | 
| `Single` | destabilizedSpringRotationMultiplier |  | 
| `Coroutine` | getUpCoroutine |  | 
| `Boolean` | grippable |  | 
| `List<RagdollHand>` | handlers |  | 
| `RagdollPart` | headPart |  | 
| `Boolean` | hipsAttached |  | 
| `Single` | hipsAttachedDamperPositionMultiplier |  | 
| `Single` | hipsAttachedDamperRotationMultiplier |  | 
| `Single` | hipsAttachedSpringPositionMultiplier |  | 
| `Single` | hipsAttachedSpringRotationMultiplier |  | 
| `IkController` | ik |  | 
| `Boolean` | isGrabbed |  | 
| `Boolean` | isTkGrabbed |  | 
| `Single` | lastCollisionEffectTime |  | 
| `Single` | lastPhysicToggleTime |  | 
| `RagdollPart` | leftUpperArmPart |  | 
| `Single` | maxPositionForce |  | 
| `Single` | maxRotationForce |  | 
| `Transform` | meshRig |  | 
| `Transform` | meshRootBone |  | 
| `HandleRagdoll` | mouthHandle |  | 
| `List<RagdollPart>` | parts |  | 
| `Single` | physicEnabledDuration |  | 
| `List<PhysicModifier>` | physicModifiers |  | 
| `Boolean` | physicToggle |  | 
| `List<Object>` | physicToggleModifiers |  | 
| `Single` | physicTogglePlayerRadius |  | 
| `Single` | physicToggleRagdollRadius |  | 
| `Single` | playerArmMaxPositionForce |  | 
| `Single` | playerArmMaxRotationForce |  | 
| `Single` | playerArmPositionDamper |  | 
| `Single` | playerArmPositionSpring |  | 
| `Single` | playerArmRotationDamper |  | 
| `Single` | playerArmRotationSpring |  | 
| `Single` | preStandUpDuration |  | 
| `Single` | preStandUpRatio |  | 
| `RagdollPart` | rightUpperArmPart |  | 
| `RagdollPart` | rootPart |  | 
| `Single` | springPositionForce |  | 
| `Single` | springRotationForce |  | 
| `Boolean` | standingUp |  | 
| `AnimationCurve` | standUpCurve |  | 
| `Single` | standUpFromGrabDuration |  | 
| `State` | state |  | 
| `RagdollPart` | targetPart |  | 
| `List<SpellCaster>` | tkHandlers |  | 
| `Single` | totalMass |  | 


Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `GrabEvent` | OnGrabEvent |  | 
| `SliceEvent` | OnSliceEvent |  | 
| `StateChange` | OnStateChange |  | 
| `TelekinesisGrabEvent` | OnTelekinesisGrabEvent |  | 
| `TelekinesisReleaseEvent` | OnTelekinesisReleaseEvent |  | 
| `UngrabEvent` | OnUngrabEvent |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddPhysicToggleModifier(`Object` handler) |  | 
| `void` | CancelGetUp() |  | 
| `void` | ClearPhysicModifiers() |  | 
| `void` | ClearPhysicToggleModifiers() |  | 
| `void` | DisableCharJointBreakForce() |  | 
| `void` | DisableJointLimit() |  | 
| `void` | EnableCharJointBreakForce(`Single` multiplier = 1) |  | 
| `void` | EnableJointLimit() |  | 
| `Transform` | FindTransformAtSamePath(`Transform` transform, `Transform` targetTransform, `Transform` targetRoot) |  | 
| `Bone` | GetBone(`Transform` meshOrAnimBone) |  | 
| `String` | GetGameObjectPath(`Transform` target, `Transform` root) |  | 
| `HandleRagdoll` | GetHandle(`String` name) |  | 
| `RagdollPart` | GetPart(`Transform` meshBone) |  | 
| `RagdollPart` | GetPart(`Type` partTypes) |  | 
| `Boolean` | GetPhysicToggle() |  | 
| `Boolean` | HasHangingItemAtProximity() |  | 
| `Boolean` | HasPenetratedObject() |  | 
| `Boolean` | HasThrowedItemAtProximity() |  | 
| `Boolean` | HasThrowedRagdollPartAtProximity() |  | 
| `Boolean` | HasTKItemAtProximity() |  | 
| `void` | IgnoreCollision(`Collider` collider, `Boolean` active, `Type` ignoredParts = 0) |  | 
| `void` | IgnoreCollision(`Ragdoll` otherRagdoll, `Boolean` active) |  | 
| `void` | Init(`Creature` creature) |  | 
| `void` | InvokeGrabEvent(`RagdollHand` ragdollHand, `HandleRagdoll` handleRagdoll) |  | 
| `void` | InvokeTelekinesisGrabEvent(`SpellTelekinesis` spellTelekinesis, `HandleRagdoll` handleRagdoll) |  | 
| `void` | InvokeTelekinesisReleaseEvent(`SpellTelekinesis` spellTelekinesis, `HandleRagdoll` handleRagdoll, `Boolean` lastHandler) |  | 
| `void` | InvokeUngrabEvent(`RagdollHand` ragdollHand, `HandleRagdoll` handleRagdoll, `Boolean` lastHandler) |  | 
| `void` | Load(`CreatureData` data) |  | 
| `void` | LoadPartsPosition() |  | 
| `void` | OnCreatureDisable() |  | 
| `void` | OnCreatureEnable() |  | 
| `void` | OnDespawn() |  | 
| `void` | OnFallEvent(`FallState` fallState) |  | 
| `void` | RefreshPartJointAndCollision() |  | 
| `void` | RefreshPartsLayer() |  | 
| `void` | RemovePhysicModifier(`Object` handler) |  | 
| `void` | RemovePhysicToggleModifier(`Object` handler) |  | 
| `void` | ResetPartsToOrigin(`Boolean` isKinematic = False) |  | 
| `void` | ResetPinForce(`Boolean` jointLimits = True, `Boolean` noRoot = False, `Type` partTypes = 0) |  | 
| `void` | SavePartsPosition() |  | 
| `void` | SetAnimationBoneToPart(`Bone` bone, `Boolean` resetNoPartBone = False) |  | 
| `void` | SetAnimationBoneToRig(`Bone` bone) |  | 
| `void` | SetAnimationBoneToRoot(`Bone` bone, `Boolean` resetToOrgPosition) |  | 
| `void` | SetBodyPositionToHead() |  | 
| `void` | SetBodyPositionToHips() |  | 
| `void` | SetColliders(`Boolean` active) |  | 
| `void` | SetMeshBone(`Bone` bone, `Boolean` forceParentMesh = False, `Boolean` parentAnimation = False) |  | 
| `void` | SetPartsLayer(`Int32` layer) |  | 
| `void` | SetPartsLayer(`LayerName` layerName) |  | 
| `void` | SetPhysicModifier(`Object` handler, `Int32` priority, `Single` gravityRatio = 1, `Single` massRatio = 1, `Single` drag = -1, `Single` angularDrag = -1, `EffectData` effectData = null) |  | 
| `void` | SetPinForce(`Single` posSpring, `Single` posDamper, `Single` rotSpring, `Single` rotDamper, `Single` posMaxForce, `Single` rotMaxForce, `Boolean` jointLimits = True, `Boolean` noRoot = False, `Type` partTypes = 0) |  | 
| `void` | SetPinForceMultiplier(`Single` springMultiplier, `Single` damperMultiplier, `Single` posMaxForceMult, `Single` rotMaxForceMult, `Boolean` jointLimits = True, `Boolean` noRoot = False, `Type` partTypes = 0) |  | 
| `void` | SetState(`State` newState, `Boolean` force = False) |  | 
| `void` | Slice(`RagdollPart` slicedPart) |  | 
| `Boolean` | SphereCastGround(`Single` sphereRadius, `Single` castLenght, `RaycastHit&` raycastHit, `Single&` groundDistance) |  | 
| `void` | StandUp() |  | 
| `IEnumerator` | StandUpCoroutine() |  | 
| `void` | UpdatePhysicToggle() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | playerPhysicBody |  | 


## `RagdollFoot`

```csharp
public class ThunderRoad.RagdollFoot
    : RagdollPart

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Transform` | grip |  | 
| `Transform` | lowerLegBone |  | 
| `PlayerFoot` | playerFoot |  | 
| `Side` | side |  | 
| `Transform` | toesAnchor |  | 
| `Transform` | toesBone |  | 
| `Transform` | upperLegBone |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | GetCurrentLegDistance(`Space` space) |  | 
| `Single` | GetLegLenght(`Space` space) |  | 
| `void` | Init() |  | 
| `void` | OnDrawGizmosSelected() |  | 
| `void` | OnValidate() |  | 


## `RagdollHand`

```csharp
public class ThunderRoad.RagdollHand
    : RagdollPart

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3` | axisPalm |  | 
| `Vector3` | axisThumb |  | 
| `SpellCaster` | caster |  | 
| `RagdollHandClimb` | climb |  | 
| `HandPose` | closePose |  | 
| `HandPoseData` | closePoseData |  | 
| `Fingers` | closePoseFingers |  | 
| `Single` | closeWeight |  | 
| `Single` | collisionUngrabMinDelay |  | 
| `Single` | collisionUngrabRadius |  | 
| `Creature` | creature |  | 
| `Handle` | disabledGrabbedHandle |  | 
| `Handle` | editorGrabTarget |  | 
| `EditPose` | editPose |  | 
| `Finger` | fingerIndex |  | 
| `Finger` | fingerLittle |  | 
| `Finger` | fingerMiddle |  | 
| `Finger` | fingerRing |  | 
| `List<Finger>` | fingers |  | 
| `Finger` | fingerThumb |  | 
| `Boolean` | forceTriggerCheck |  | 
| `Boolean` | globalRatio |  | 
| `Handle` | grabbedHandle |  | 
| `Transform` | grip |  | 
| `GripInfo` | gripInfo |  | 
| `Coroutine` | handOverlapCoroutine |  | 
| `Single` | indexCloseWeight |  | 
| `Boolean` | indexPositionReached |  | 
| `Boolean` | isHandlingSameObject |  | 
| `Single` | littleCloseWeight |  | 
| `Boolean` | littlePositionReached |  | 
| `RagdollPart` | lowerArmPart |  | 
| `Boolean` | meshFixedScale |  | 
| `Vector3` | meshGlobalScale |  | 
| `Single` | middleCloseWeight |  | 
| `Boolean` | middlePositionReached |  | 
| `Coroutine` | moveToFingerPoseCoroutine |  | 
| `Interactable` | nearestInteractable |  | 
| `HandPose` | openPose |  | 
| `HandPoseData` | openPoseData |  | 
| `Fingers` | openPoseFingers |  | 
| `Vector3` | orgGripLocalPosition |  | 
| `Quaternion` | orgGripLocalRotation |  | 
| `RagdollHand` | otherHand |  | 
| `Collider` | palmCollider |  | 
| `PlayerHand` | playerHand |  | 
| `Single` | ringCloseWeight |  | 
| `Boolean` | ringPositionReached |  | 
| `Side` | side |  | 
| `Collider` | simplifiedCollider |  | 
| `Single` | thumbCloseWeight |  | 
| `Boolean` | thumbPositionReached |  | 
| `Collider` | touchCollider |  | 
| `List<Interactable>` | touchedInteractables |  | 
| `RagdollPart` | upperArmPart |  | 
| `WristStats` | wristStats |  | 


Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `GrabEvent` | OnGrabEvent |  | 
| `UnGrabEvent` | OnUnGrabEvent |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AttachFingerMeshBoneToRagdoll() |  | 
| `void` | Awake() |  | 
| `void` | ClearTouch() |  | 
| `Transform` | CreateDefaultGrip() |  | 
| `void` | EditorGrab() |  | 
| `void` | EditorUngrab() |  | 
| `void` | FixedUpdate() |  | 
| `Single` | GetArmLenghtRatio(`Boolean` XZOnly) |  | 
| `void` | Grab(`Handle` handle) |  | 
| `void` | Grab(`Handle` handle, `Boolean` teleportToHand = False) |  | 
| `void` | Grab(`Handle` handle, `HandleOrientation` orientation, `Single` axisPosition, `Boolean` teleportToHand = False) |  | 
| `void` | GrabRelative(`Handle` handle) |  | 
| `void` | Init(`Ragdoll` ragdoll) |  | 
| `void` | InitAfterBoneInit() |  | 
| `void` | Load() |  | 
| `void` | MirrorFingersToOtherHand() |  | 
| `void` | OnCollisionEnter(`Collision` collision) |  | 
| `void` | OnCollisionStay(`Collision` collision) |  | 
| `void` | OnDrawGizmosSelected() |  | 
| `void` | OnRagdollDisable() |  | 
| `void` | OnRagdollEnable() |  | 
| `void` | OnRagdollStateChange(`State` previousState, `State` newState, `PhysicStateChange` physicStateChange, `EventTime` eventTime) |  | 
| `void` | OnValidate() |  | 
| `void` | RefreshTwoHanded() |  | 
| `void` | ResetGripPositionAndRotation() |  | 
| `void` | SaveCurrentToPose(`HandPose` handPose) |  | 
| `void` | SaveFinger(`Finger` poseFinger, `Finger` finger) |  | 
| `void` | SetClosePose(`HandPoseData` handPoseData = null) |  | 
| `void` | SetCloseWeight(`Single` weight) |  | 
| `void` | SetFingerColliders(`Boolean` enabled) |  | 
| `void` | SetGripFromClosePose() |  | 
| `void` | SetGripFromOpenPose() |  | 
| `void` | SetGripToDefaultPosition() |  | 
| `void` | SetOpenPose(`HandPoseData` handPoseData = null) |  | 
| `void` | SetupFinger(`Finger` finger, `String` name) |  | 
| `void` | SetupFingers() |  | 
| `Boolean` | TouchedInteractablesContain(`Interactable` interactable) |  | 
| `Boolean` | TryAction(`Action` action) |  | 
| `Boolean` | TryRelease() |  | 
| `void` | UnGrab(`Boolean` throwing) |  | 
| `void` | UpdateClimb() |  | 
| `void` | UpdateFinger(`Finger` finger, `Finger` openPoseFinger, `Finger` closePoseFinger, `Single` ratio) |  | 
| `void` | UpdatePlayerPose() |  | 
| `void` | UpdatePoseIndex(`Single` weight) |  | 
| `void` | UpdatePoseLittle(`Single` weight) |  | 
| `void` | UpdatePoseMiddle(`Single` weight) |  | 
| `void` | UpdatePoseRing(`Single` weight) |  | 
| `void` | UpdatePoseThumb(`Single` weight) |  | 


## `RagdollHandClimb`

```csharp
public class ThunderRoad.RagdollHandClimb

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `SphereCollider` | gripHandCollider |  | 
| `Item` | gripItem |  | 
| `Transform` | gripNode |  | 
| `GripRayCast` | gripRayCast |  | 
| `Rigidbody` | gripRb |  | 
| `Boolean` | gripRbIsTemp |  | 
| `Boolean` | indexContact |  | 
| `Collider` | indexContactCollider |  | 
| `Boolean` | isGripping |  | 
| `Int32` | justGrabbed |  | 
| `Boolean` | littleContact |  | 
| `Collider` | littleContactCollider |  | 
| `Boolean` | middleContact |  | 
| `Collider` | middleContactCollider |  | 
| `PhysicMaterial` | orgMaterial |  | 
| `Boolean` | palmContact |  | 
| `Collider` | palmContactCollider |  | 
| `RagdollHand` | ragdollHand |  | 
| `Boolean` | ringContact |  | 
| `Collider` | ringContactCollider |  | 
| `Coroutine` | throwCoroutine |  | 
| `Boolean` | thumbContact |  | 
| `Collider` | thumbContactCollider |  | 
| `Boolean` | wasGrabbed |  | 
| `Boolean` | wasJumping |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CheckColliderBetweenFingers(`Collider` collider, `Bone` finger1, `Bone` finger2) |  | 
| `Boolean` | CheckColliderBetweenPalm(`Collider` collider, `Bone` finger) |  | 
| `Boolean` | CheckFingerBoneOverlap(`Bone` fingerBone) |  | 
| `Boolean` | CheckFingerContact(`Finger` finger, `Collider` collider) |  | 
| `Boolean` | CheckFingerOverlap(`Finger` finger) |  | 
| `void` | CheckFingersContact(`ContactPoint` contactPoint) |  | 
| `void` | CheckFingersOverlap() |  | 
| `void` | CleanDummyHand(`Item` item) |  | 
| `void` | CreateDummyHandOnObject(`Item` item) |  | 
| `void` | FixedUpdate() |  | 
| `void` | OnCollisionEnter(`Collision` collision) |  | 
| `void` | OnCollisionStay(`Collision` collision) |  | 
| `void` | OnTriggerEnter(`Collider` collider) |  | 
| `void` | OnTriggerStay(`Collider` collider) |  | 
| `void` | TryGrip() |  | 
| `void` | UnGrip() |  | 
| `void` | Update() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | climbFree |  | 
| `String` | dummyLeftColliderName |  | 
| `String` | dummyRightColliderName |  | 
| `Boolean` | holdGrip |  | 


## `RagdollPart`

```csharp
public class ThunderRoad.RagdollPart
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Damager` | bodyDamager |  | 
| `Boolean` | bodyDamagerIsAttack |  | 
| `Bone` | bone |  | 
| `Vector3` | boneToChildDirection |  | 
| `CharacterJoint` | characterJoint |  | 
| `Boolean` | characterJointLocked |  | 
| `ColliderGroup` | colliderGroup |  | 
| `CollisionHandler` | collisionHandler |  | 
| `Single` | damperPositionMultiplier |  | 
| `Single` | damperRotationMultiplier |  | 
| `PartData` | data |  | 
| `List<HandleRagdoll>` | handles |  | 
| `List<RagdollPart>` | ignoredParts |  | 
| `Boolean` | ignoreStaticCollision |  | 
| `Boolean` | initialized |  | 
| `Boolean` | isGrabbed |  | 
| `Boolean` | isSliced |  | 
| `Transform[]` | linkedMeshBones |  | 
| `Transform` | meshBone |  | 
| `CharacterJointData` | orgCharacterJointData |  | 
| `RagdollPart` | parentPart |  | 
| `Ragdoll` | ragdoll |  | 
| `Rigidbody` | rb |  | 
| `List<RendererData>` | renderers |  | 
| `Boolean` | ripBreak |  | 
| `Single` | ripBreakForce |  | 
| `Transform` | root |  | 
| `Vector3` | rootOrgLocalPosition |  | 
| `Quaternion` | rootOrgLocalRotation |  | 
| `Vector3` | savedPosition |  | 
| `Quaternion` | savedRotation |  | 
| `Boolean` | sliceAllowed |  | 
| `RagdollPart` | sliceChildAndDisableSelf |  | 
| `Transform` | slicedMeshRoot |  | 
| `Material` | sliceFillMaterial |  | 
| `Single` | sliceHeight |  | 
| `Single` | sliceParentAdjust |  | 
| `Single` | sliceThreshold |  | 
| `Single` | sliceWidth |  | 
| `Single` | springPositionMultiplier |  | 
| `Single` | springRotationMultiplier |  | 
| `Type` | type |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | CreateCharJoint(`Boolean` resetPosition) |  | 
| `void` | DestroyCharJoint() |  | 
| `void` | DisableCharJointLimit() |  | 
| `void` | EnableCharJointBreakForce(`Single` multiplier = 1) |  | 
| `void` | FindBoneFromName() |  | 
| `void` | FixedCharJointLimit() |  | 
| `Single` | GetPinDamperPosition() |  | 
| `Single` | GetPinDamperRotation() |  | 
| `Single` | GetPinSpringPosition() |  | 
| `Single` | GetPinSpringRotation() |  | 
| `Vector3` | GetSliceDirection() |  | 
| `void` | GetSlicePositionAndDirection(`Vector3&` position, `Vector3&` direction) |  | 
| `Boolean` | HasCollider(`Collider` collider) |  | 
| `void` | Init(`Ragdoll` ragdoll) |  | 
| `void` | Load() |  | 
| `void` | OnDrawGizmosSelected() |  | 
| `void` | OnJointBreak() |  | 
| `void` | OnRagdollDisable() |  | 
| `void` | OnRagdollEnable() |  | 
| `void` | OnValidate() |  | 
| `void` | RefreshLayer() |  | 
| `void` | ResetCharJointBreakForce() |  | 
| `void` | ResetCharJointLimit() |  | 
| `void` | SetBodyDamagerToAttack() |  | 
| `void` | SetBodyDamagerToDefault() |  | 
| `void` | SetLayer(`Int32` layer) |  | 
| `void` | SetLayer(`LayerName` layerName) |  | 
| `void` | SetPositionToBone() |  | 
| `void` | Slice() |  | 
| `void` | UpdateRenderers() |  | 


## `RagdollTester`

```csharp
public class ThunderRoad.RagdollTester
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Transform` | animatorRig |  | 
| `List<Bone>` | bones |  | 
| `Creature` | creature |  | 
| `List<RagdollPart>` | parts |  | 
| `Ragdoll` | ragdoll |  | 
| `State` | state |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DisableJointLimit() |  | 
| `void` | EnableJointLimit() |  | 
| `Transform` | FindTransformAtSamePath(`Transform` transform, `Transform` targetTransform, `Transform` targetRoot) |  | 
| `Bone` | GetBone(`Transform` meshOrAnimBone) |  | 
| `String` | GetGameObjectPath(`Transform` target, `Transform` root) |  | 
| `RagdollPart` | GetPart(`Transform` meshBone) |  | 
| `void` | SetAnimationBoneToPart(`Bone` bone) |  | 
| `void` | SetAnimationBoneToRig(`Bone` bone) |  | 
| `void` | SetAnimationBoneToRoot(`Bone` bone) |  | 
| `void` | SetMeshBone(`Bone` bone, `Boolean` forceParentMesh = False) |  | 
| `void` | SetState(`State` newState) |  | 
| `void` | SetStateToDestabilized() |  | 
| `void` | SetStateToFrozen() |  | 
| `void` | SetStateToFullAttached() |  | 
| `void` | SetStateToHipsAttached() |  | 
| `void` | SetStateToInert() |  | 
| `void` | SetStateToNoPhysics() |  | 


## `RawImageFiller`

```csharp
public class ThunderRoad.RawImageFiller
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | addressableTexture |  | 
| `UIItemSpawner` | inventory |  | 
| `RawImage` | rawImage |  | 
| `Value` | value |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnDisable() |  | 
| `void` | OnEnable() |  | 


## `RenderCubemap`

```csharp
public class ThunderRoad.RenderCubemap
    : MonoBehaviour

```

## `RepulsionForce`

```csharp
public class ThunderRoad.RepulsionForce
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | colliderCount |  | 
| `Collider[]` | colliders |  | 
| `Single` | force |  | 
| `Single` | radius |  | 


## `RevealDecal`

```csharp
public class ThunderRoad.RevealDecal
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `RevealMaskResolution` | maskHeight |  | 
| `RevealMaskResolution` | maskWidth |  | 
| `RevealMaterialController` | revealMaterialController |  | 
| `Type` | type |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ActivateReveal() |  | 
| `void` | Blit(`Single` multiplier = 0.1) |  | 
| `void` | Reset() |  | 
| `void` | SetMaskResolution(`Single` scale = 1) |  | 
| `void` | SetMaskResolutionEighth() |  | 
| `void` | SetMaskResolutionFull() |  | 
| `void` | SetMaskResolutionHalf() |  | 
| `void` | SetMaskResolutionQuarter() |  | 
| `Boolean` | UpdateOvertime() |  | 


## `RevealMaskTester`

```csharp
public class ThunderRoad.RevealMaskTester
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BlendOp` | blitBlendOp |  | 
| `ColorWriteMask` | blitColorWriteMask |  | 
| `Single` | blitDuration |  | 
| `Vector4` | blitMultiplier |  | 
| `Single` | blitStep |  | 
| `Vector4` | channelMultiplier |  | 
| `Boolean` | continuous |  | 
| `Damage` | damage |  | 
| `RevealDataAsset` | defaultBlunt |  | 
| `RevealDataAsset` | defaultBluntFire |  | 
| `Single` | defaultMaxSize |  | 
| `Single` | defaultMinSize |  | 
| `RevealDataAsset` | defaultPierce |  | 
| `RevealDataAsset` | defaultPierceFire |  | 
| `RevealDataAsset` | defaultSlash |  | 
| `RevealDataAsset` | defaultSlashFire |  | 
| `Single` | depth |  | 
| `List<IdmapReveal>` | idmapReveals |  | 
| `Boolean` | isFire |  | 
| `Color` | lastIdMapColor |  | 
| `Single` | offset |  | 
| `Boolean` | randomRotation |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Blit() |  | 
| `void` | BlitSkinShaderOnly() |  | 
| `void` | OnProjectCompleted(`Single` overTime) |  | 
| `void` | ResetLastHit() |  | 


## `RewardItem`

```csharp
public class ThunderRoad.RewardItem
    : MonoBehaviour

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | InitItem(`LevelModuleSurvival` aLevelModuleSurvival) |  | 


## `Room`

```csharp
public class ThunderRoad.Room
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<AudioSource>` | audioSourcesToBlend |  | 
| `Boolean` | autoRotateDirLight |  | 
| `List<BlendAudioSource>` | blendAudioSources |  | 
| `Boolean` | changeFogColor |  | 
| `Boolean` | changeShadowColor |  | 
| `List<Creature>` | creatures |  | 
| `PerfectCullingVolume` | cullingVolume |  | 
| `Light` | directionalLight |  | 
| `Quaternion` | directionalLightRotation |  | 
| `Color` | dirLightColor |  | 
| `Single` | dirLightIndirectMultiplier |  | 
| `Single` | dirLightIntensity |  | 
| `List<DungeonDoor>` | doors |  | 
| `DungeonDoor` | entryDoor |  | 
| `DungeonDoor` | exitDoor |  | 
| `Color` | fogColor |  | 
| `Int32` | index |  | 
| `Boolean` | initialized |  | 
| `Boolean` | isCulled |  | 
| `Boolean` | isHidden |  | 
| `List<Item>` | items |  | 
| `Int32` | maxItems |  | 
| `Int32` | maxItemsAndroid |  | 
| `Room` | next |  | 
| `UnityEvent` | onPlayerEnter |  | 
| `UnityEvent` | onPlayerExit |  | 
| `List<ParticleSystem>` | particleSystems |  | 
| `List<PlayerSpawner>` | playerSpawners |  | 
| `Room` | previous |  | 
| `RoomProxy` | proxy |  | 
| `List<ReflectionProbe>` | reflectionProbes |  | 
| `GameObject` | rootNoCulling |  | 
| `Color` | shadowColor |  | 
| `Boolean` | shareAlertBetweenNPC |  | 
| `Int32` | spawnerMaxNPC |  | 
| `Int32` | spawnerNPCCount |  | 
| `Single` | spawnRoomObjectsAcrossFrames |  | 
| `Tile` | tile |  | 
| `Coroutine` | toggleRoomObjectCoroutine |  | 
| `List<VisualEffect>` | visualEffects |  | 
| `List<VolumetricLightBeam>` | volumetricLightBeams |  | 


Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `VisibilityChangeEvent` | onVisibilityChange |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | Contains(`Vector3` position) |  | 
| `Light` | GetDirectionalLight() |  | 
| `PlayerSpawner` | GetPlayerSpawner() |  | 
| `void` | Hide(`Boolean` hide) |  | 
| `void` | InitReflectionProbeRotation(`ReflectionProbe` reflectionProbe) |  | 
| `Boolean` | IsAdditionalNonLOD0Collider(`LODGroup` lODGroup, `Collider` collider) |  | 
| `Boolean` | LODHaveRenderers(`LOD` lod) |  | 
| `void` | OnPlayerEnter() |  | 
| `void` | OnPlayerExit() |  | 
| `void` | RegisterCreature(`Creature` creature) |  | 
| `void` | RegisterItem(`Item` item) |  | 
| `void` | SaveSceneDirectionalLightRotation() |  | 
| `void` | SetCull(`Boolean` cull) |  | 
| `void` | SetSceneDirectionalLightRotation() |  | 
| `void` | StaticBatch() |  | 
| `void` | UnRegisterCreature(`Creature` creature) |  | 
| `void` | UnRegisterItem(`Item` item) |  | 


## `RoomProxy`

```csharp
public class ThunderRoad.RoomProxy
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Doorway>` | doorways |  | 
| `AssetReferenceGameObject` | roomPrefab |  | 
| `AssetReferenceGameObject` | roomPrefabAndroid |  | 
| `Boolean` | spawnCreature |  | 
| `Tile` | tile |  | 


## `Rope`

```csharp
public class ThunderRoad.Rope
    : Handle

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | dynamicHeight |  | 
| `Single` | heightFromGround |  | 
| `Interactable` | interactable |  | 
| `Single` | raycastRange |  | 
| `Int32` | ropeLayer |  | 
| `Material` | ropeMaterial |  | 
| `PhysicMaterial` | ropePhysicMaterial |  | 
| `Single` | ropeRadius |  | 
| `Transform` | ropeStart |  | 
| `Transform` | ropeTarget |  | 
| `Boolean` | ropeUseCollider |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | Generate() |  | 
| `List<ValueDropdownItem<String>>` | GetAllInteractableID() |  | 
| `void` | OnDrawGizmos() |  | 
| `void` | Start() |  | 


## `RopeSimple`

```csharp
public class ThunderRoad.RopeSimple
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | audioMaxForce |  | 
| `Single` | audioMaxSpeed |  | 
| `Single` | audioMinForce |  | 
| `Single` | audioMinSpeed |  | 
| `Single` | damper |  | 
| `String` | effectId |  | 
| `Material` | material |  | 
| `Single` | maxDistance |  | 
| `Single` | minDistance |  | 
| `Single` | radius |  | 
| `Single` | spring |  | 
| `Transform` | targetAnchor |  | 
| `Single` | tilingOffset |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `List<ValueDropdownItem<String>>` | GetAllEffectID() |  | 
| `void` | LateUpdate() |  | 
| `void` | OnDisable() |  | 
| `void` | OnDrawGizmos() |  | 


## `RotateToVelocity`

```csharp
public class ThunderRoad.RotateToVelocity
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3` | defaultDirection |  | 
| `Single` | maxSpeed |  | 
| `Single` | minSpeed |  | 
| `Boolean` | revert |  | 
| `Rigidbody` | rigidbody |  | 
| `Vector3` | upwards |  | 


## `SavedValueID`

```csharp
public enum ThunderRoad.SavedValueID
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | Rack |  | 
| `1` | Holder |  | 
| `2` | PotionFill |  | 
| `3` | Ammo |  | 
| `4` | LevelCastThrow |  | 
| `5` | LevelCastSpray |  | 
| `6` | LevelCharge |  | 
| `7` | LevelImbue |  | 
| `8` | LevelMergeAppart |  | 
| `9` | LevelMergeUp |  | 
| `10` | LevelMergeForward |  | 
| `11` | LevelMergeDown |  | 
| `12` | LevelCrystalShockwave |  | 
| `13` | LevelCrystalForward |  | 
| `14` | LevelCrystalFire |  | 
| `15` | Grab |  | 


## `ShootPoint`

```csharp
public class ThunderRoad.ShootPoint
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | allowedAngle |  | 
| `Creature` | currentCreature |  | 
| `Vector3` | navPosition |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnDrawGizmos() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<ShootPoint>` | list |  | 


## `ShootPosition`

```csharp
public class ThunderRoad.ShootPosition

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Creature` | creature |  | 
| `Vector3` | position |  | 
| `Boolean` | valid |  | 


## `Side`

```csharp
public enum ThunderRoad.Side
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | Right |  | 
| `1` | Left |  | 


## `SkillData`

```csharp
public class ThunderRoad.SkillData
    : CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String[]` | dependancies |  | 
| `SkillData[]` | dependantSkills |  | 
| `Int32` | depth |  | 
| `String` | description |  | 
| `String` | displayName |  | 
| `Texture` | image |  | 
| `String` | imageAddress |  | 
| `EffectData` | orbLinkEffectData |  | 
| `String` | orbLinkEffectId |  | 
| `String` | prefabAddress |  | 
| `String` | treeName |  | 
| `Int32` | upgrades |  | 
| `VideoClip` | video |  | 
| `String` | videoAddress |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<ValueDropdownItem<String>>` | GetAllEffectID() |  | 
| `List<ValueDropdownItem<String>>` | GetAllSkillID() |  | 
| `void` | OnCatalogRefresh() |  | 


## `SkillTree`

```csharp
public class ThunderRoad.SkillTree
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Coroutine` | checkCrossDependanciesCoroutine |  | 
| `Single` | circleRadius |  | 
| `Single` | colorChangeSpeed |  | 
| `Single` | crossOuterDistance |  | 
| `List<SkillTreeOrb>` | crossSkillOrbs |  | 
| `Boolean` | crystalChangeRingColor |  | 
| `Color` | crystalCumulativeEmissionColor |  | 
| `Single` | floorHeight |  | 
| `Single` | hideTreeDuration |  | 
| `Renderer` | monolith |  | 
| `Color` | monolithEmissionColor |  | 
| `Single` | positionDamper |  | 
| `Single` | positionMaxForce |  | 
| `Single` | positionSpring |  | 
| `List<SkillTreeReceptacle>` | receptacles |  | 
| `Single` | ringAutoRotationPlayerDistance |  | 
| `Single` | ringAutoRotationTargetVelocity |  | 
| `Color` | ringCurrentEmissionColor |  | 
| `Color` | ringEmissionColor |  | 
| `HingeJoint` | ringJoint |  | 
| `JointMotor` | ringJointMotor |  | 
| `MaterialPropertyBlock` | ringMaterialPropertyBlock |  | 
| `Renderer` | ringMedium |  | 
| `Renderer` | ringReceptacles |  | 
| `Single` | ringRotationForce |  | 
| `Single` | ringRotationTargetVelocity |  | 
| `Single` | ringSleepThreshold |  | 
| `Renderer` | ringSmall |  | 
| `Single` | rotationDamper |  | 
| `Single` | rotationMaxForce |  | 
| `Single` | rotationSpring |  | 
| `Single` | showTreeDelay |  | 
| `Single` | showTreeDuration |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CheckCrossDependancies() |  | 
| `List<SkillTreeOrb>` | GetExistingLinkedOrbs(`SkillData` skillData) |  | 


## `SkillTreeCrystal`

```csharp
public class ThunderRoad.SkillTreeCrystal
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Item` | item |  | 
| `SkillTreeReceptacle` | receptacle |  | 
| `Color` | skilltreeEmissionColor |  | 
| `String` | treeName |  | 


## `SkillTreeOrb`

```csharp
public class ThunderRoad.SkillTreeOrb
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Rigidbody` | anchor |  | 
| `SkillData` | data |  | 
| `List<SkillTreeOrb>` | dependancies |  | 
| `List<EffectInstance>` | effectInstanceLinks |  | 
| `ConfigurableJoint` | joint |  | 
| `MeshRenderer` | orbRenderer |  | 
| `Rigidbody` | rb |  | 
| `SkillTreeReceptacle` | receptacle |  | 
| `SkillTree` | skillTree |  | 
| `SphereCollider` | sphereCollider |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Init(`SkillData` data, `SkillTree` skillTree, `SkillTreeReceptacle` skillTreeReceptacle = null) |  | 
| `void` | RefreshJoint() |  | 


## `SkillTreeReceptacle`

```csharp
public class ThunderRoad.SkillTreeReceptacle
    : ItemMagnet

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Collider>` | colliders |  | 
| `Coroutine` | hideTreeCoroutine |  | 
| `Renderer` | mesh |  | 
| `Coroutine` | showTreeCoroutine |  | 
| `SkillTree` | skillTree |  | 
| `SkillTreeCrystal` | skillTreeCrystal |  | 
| `List<SkillTreeOrb>` | skillTreeOrbs |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | HideTree() |  | 
| `void` | OnItemCatch(`Item` item, `EventTime` eventTime) |  | 
| `void` | OnItemRelease(`Item` item, `EventTime` eventTime) |  | 
| `void` | OnValidate() |  | 
| `void` | ShowTree() |  | 


## `SkyDome`

```csharp
public class ThunderRoad.SkyDome
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | active |  | 
| `GameObject` | aurora |  | 
| `Camera` | cam |  | 
| `UniversalAdditionalCameraData` | cameraData |  | 
| `GameObject` | cloud |  | 
| `GameObject` | jovian |  | 
| `GameObject` | neutronStar |  | 
| `Camera` | playerCamera |  | 
| `UniversalAdditionalCameraData` | playerCameraData |  | 
| `GameObject` | rings |  | 
| `Single` | skyboxHorizontalAngle |  | 
| `GameObject` | stars |  | 
| `GameObject` | sun |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnBeforeRender() |  | 
| `void` | OnDisable() |  | 
| `void` | OnEnable() |  | 
| `void` | OnUserPresenceChange() |  | 
| `void` | SetCamera(`Boolean` active) |  | 
| `void` | SetRotation(`Single` rotationY) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `SkyDome` | instance |  | 


## `SliceTester`

```csharp
public class ThunderRoad.SliceTester
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Transform[]` | bonesToRip |  | 
| `Transform` | boneToRip |  | 
| `GameObject` | meshRoot |  | 
| `Material` | sliceFill |  | 
| `Single` | threshold |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Slice() |  | 


## `Slider`

```csharp
public class ThunderRoad.Slider
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Button` | btnNext |  | 
| `Button` | btnPrevious |  | 
| `RawImage` | colorViewer |  | 
| `RawImage` | colorViewer2 |  | 
| `Single` | increment |  | 
| `Single` | maxValue |  | 
| `Single` | minValue |  | 
| `Slider` | slider |  | 
| `Text` | title |  | 
| `Text` | value |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | InitValues() |  | 
| `void` | LoadValue() |  | 
| `void` | NextValue() |  | 
| `void` | OnBeginDrag(`PointerEventData` eventData) |  | 
| `void` | OnDrag(`PointerEventData` data) |  | 
| `void` | OnEnable() |  | 
| `void` | OnEndDrag(`PointerEventData` data) |  | 
| `void` | OnSliderValueChanged() |  | 
| `void` | OnValidate() |  | 
| `void` | PreviousValue() |  | 
| `void` | Refresh() |  | 
| `void` | RefreshDisplay() |  | 
| `void` | SetInteractable(`Boolean` active) |  | 
| `void` | Start() |  | 


## `SliderCreatureRGB`

```csharp
public class ThunderRoad.SliderCreatureRGB
    : SliderRGB, IEndDragHandler, IEventSystemHandler

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Creature` | creature |  | 
| `SharedColor` | umaColor |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnEnable() |  | 
| `void` | OnEndDrag(`PointerEventData` data) |  | 
| `void` | Refresh() |  | 


## `SliderDifficulty`

```csharp
public class ThunderRoad.SliderDifficulty
    : Slider

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | OnEnable() |  | 
| `void` | OnEndDrag(`PointerEventData` data) |  | 
| `void` | OnSliderValueChanged() |  | 
| `void` | OnValidate() |  | 
| `void` | Refresh() |  | 
| `void` | SetNames(`String[]` someNames, `String[]` someDescriptions) |  | 


## `SliderDNA`

```csharp
public class ThunderRoad.SliderDNA
    : Slider

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Creature` | creature |  | 
| `DNA` | DNAProperty |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | InitValues() |  | 
| `void` | LoadValue() |  | 
| `void` | OnEndDrag(`PointerEventData` data) |  | 
| `void` | OnSliderValueChanged() |  | 
| `void` | RefreshDisplay() |  | 


## `SliderDragEvent`

```csharp
public class ThunderRoad.SliderDragEvent
    : MonoBehaviour, IBeginDragHandler, IEventSystemHandler, IDragHandler, IEndDragHandler

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnBeginDrag(`PointerEventData` eventData) |  | 
| `void` | OnDrag(`PointerEventData` eventData) |  | 
| `void` | OnEndDrag(`PointerEventData` eventData) |  | 


## `SliderOptions`

```csharp
public class ThunderRoad.SliderOptions
    : Slider

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Option` | option |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | InitValues() |  | 
| `void` | LoadValue() |  | 
| `void` | OnEndDrag(`PointerEventData` data) |  | 
| `void` | OnSliderValueChanged() |  | 
| `void` | RefreshDisplay() |  | 


## `SliderRGB`

```csharp
public class ThunderRoad.SliderRGB
    : MonoBehaviour, IEndDragHandler, IEventSystemHandler

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `RawImage` | colorViewer |  | 
| `Single` | maxRgb |  | 
| `Slider` | sliderB |  | 
| `Slider` | sliderG |  | 
| `Slider` | sliderR |  | 
| `Text` | title |  | 
| `Text` | valueB |  | 
| `Text` | valueG |  | 
| `Text` | valueR |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | OnEnable() |  | 
| `void` | OnEndDrag(`PointerEventData` data) |  | 
| `void` | onValueChanged(`RGB` rgb) |  | 


## `Spectator`

```csharp
public class ThunderRoad.Spectator
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<GameObject>` | arcadeVersion |  | 
| `List<GameObject>` | AutoCamText |  | 
| `Camera` | cam |  | 
| `Boolean` | cameraStabilization |  | 
| `Single` | cameraStabilizationSpeed |  | 
| `Canvas` | canvas |  | 
| `Boolean` | debugConsoleShown |  | 
| `DebugLogManager` | debugLogManager |  | 
| `String` | debugLogManagerAddress |  | 
| `Single` | defaultFov |  | 
| `List<GameObject>` | defaultVersion |  | 
| `List<GameObject>` | FreeCamText |  | 
| `Single` | gamepadRotationSpeed |  | 
| `GameObject` | help |  | 
| `InputSystemUIInputModule` | inputSystemUIInputModule |  | 
| `Boolean` | isPanelOpen |  | 
| `Single` | lastMouseUsedTime |  | 
| `Dropdown` | levelDropdown |  | 
| `Vector3` | lockedLocalPosition |  | 
| `Quaternion` | lockedLocalRotation |  | 
| `Transform` | lockedTransform |  | 
| `Single` | lockRadius |  | 
| `GameObject` | logo |  | 
| `Boolean` | motionBlur |  | 
| `Boolean` | mouseUsed |  | 
| `Single` | movementSpeed |  | 
| `Single` | movementSpeedChange |  | 
| `GameObject` | panel |  | 
| `RectTransform` | panelName |  | 
| `InputField` | playerNameInputField |  | 
| `GameObject` | rendererGameObject |  | 
| `Single` | rotationSpeed |  | 
| `Transform` | shootTransform |  | 
| `Boolean` | showHelp |  | 
| `Boolean` | showLogo |  | 
| `State` | state |  | 
| `Toggle` | toggleAllowBloodEffects |  | 
| `Toggle` | toggleFallDamage |  | 
| `Toggle` | toggleInfiniteArrows |  | 
| `Toggle` | toggleInfiniteFocus |  | 
| `Toggle` | toggleInfiniteImbue |  | 
| `Toggle` | toggleInfiniteMana |  | 
| `Toggle` | toggleInvincibility |  | 
| `Toggle` | toggleMotionBlur |  | 
| `Toggle` | toggleShowHelp |  | 
| `Toggle` | toggleShowLogo |  | 
| `Toggle` | toggleStabilization |  | 
| `Toggle` | toggleViewAuto |  | 
| `Toggle` | toggleViewFpv |  | 
| `Toggle` | toggleViewFree |  | 
| `Toggle` | toggleViewHMD |  | 
| `Slider` | viewFovSlider |  | 
| `GameObject` | viewWarningPerf |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `IEnumerator` | DebugConsoleCoroutine() |  | 
| `void` | OnDebugOptionChanged(`Parameter` parameter) |  | 
| `void` | OnPlayerSpawned(`Player` player) |  | 
| `void` | RefreshDebugOptions() |  | 
| `void` | SavePlayerName() |  | 
| `void` | SetFov(`Single` fov) |  | 
| `void` | SetInputModule(`Boolean` active) |  | 
| `void` | SetMotionBlur(`Boolean` active) |  | 
| `void` | SetStabilization(`Boolean` active) |  | 
| `void` | SetViewAuto() |  | 
| `void` | SetViewFPV() |  | 
| `void` | SetViewFree() |  | 
| `void` | SetViewHmd() |  | 
| `void` | Shoot() |  | 
| `void` | ShowDebugConsole(`Boolean` show) |  | 
| `void` | ShowHelp(`Boolean` active) |  | 
| `void` | ShowLogo(`Boolean` active) |  | 
| `void` | ShowPanel(`Boolean` active) |  | 
| `void` | ShowPanelName(`Boolean` mustShow) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | forceStateOnStart |  | 
| `Spectator` | local |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | SetDisplayCameraToAllCanvas() |  | 


## `SpellCastCharge`

```csharp
public class ThunderRoad.SpellCastCharge
    : SpellCastData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | allowSpray |  | 
| `Boolean` | allowThrow |  | 
| `EffectData` | chargeEffectData |  | 
| `String` | chargeEffectId |  | 
| `EffectInstance` | chargeEffectInstance |  | 
| `Single` | chargeMaxHaptic |  | 
| `Single` | chargeMinHaptic |  | 
| `Single` | chargeSpeed |  | 
| `HandPoseData` | closeHandPoseData |  | 
| `String` | closeHandPoseId |  | 
| `Single` | currentCharge |  | 
| `EffectData` | fingerEffectData |  | 
| `String` | fingerEffectId |  | 
| `Single` | grabbedFireMaxCharge |  | 
| `Imbue` | imbue |  | 
| `Boolean` | imbueAllowMetal |  | 
| `EffectData` | imbueBladeEffectData |  | 
| `String` | imbueBladeEffectId |  | 
| `EffectData` | imbueCrystalEffectData |  | 
| `String` | imbueCrystalEffectId |  | 
| `EffectInstance` | imbueEffect |  | 
| `Boolean` | imbueEnabled |  | 
| `Single` | imbueHitMinVelocity |  | 
| `Boolean` | imbueHitUseDamager |  | 
| `Single` | imbueManaConsumption |  | 
| `EffectData` | imbueMetalEffectData |  | 
| `String` | imbueMetalEffectId |  | 
| `Single` | imbueRadius |  | 
| `Single` | imbueRate |  | 
| `EffectData` | imbueTransferEffectData |  | 
| `String` | imbueTransferEffectId |  | 
| `Single` | imbueWhooshHapticMultiplier |  | 
| `Single` | imbueWhooshMaxSpeed |  | 
| `Single` | imbueWhooshMinSpeed |  | 
| `Boolean` | isCustomImbue |  | 
| `Boolean` | isSpraying |  | 
| `HandPoseData` | openHandPoseData |  | 
| `String` | openHandPoseId |  | 
| `SpellCaster` | spellCaster |  | 
| `HandPoseData` | sprayHandPoseData |  | 
| `String` | sprayHandPoseId |  | 
| `Single` | sprayHeadToFireMaxAngle |  | 
| `Vector3` | sprayMagicOffset |  | 
| `Single` | sprayMinCharge |  | 
| `Boolean` | stopIfManaDepleted |  | 
| `Single` | stopSpeed |  | 
| `EffectData` | throwEffectData |  | 
| `String` | throwEffectId |  | 
| `Single` | throwMinCharge |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `SpellCastCharge` | Clone() |  | 
| `void` | Fire(`Boolean` active) |  | 
| `void` | FireAxis(`Single` value) |  | 
| `List<ValueDropdownItem<String>>` | GetAllEffectID() |  | 
| `List<ValueDropdownItem<String>>` | GetAllHandPoseID() |  | 
| `Int32` | GetCurrentVersion() |  | 
| `void` | Load(`SpellCaster` spellCaster, `Level` level) |  | 
| `void` | Load(`Imbue` imbue, `Level` level) |  | 
| `void` | OnCatalogRefresh() |  | 
| `void` | OnCrystalUse(`Side` side, `Boolean` active) |  | 
| `void` | OnImbueCollisionStart(`CollisionInstance` collisionInstance) |  | 
| `void` | OnImbueCollisionStop(`CollisionInstance` collisionInstance) |  | 
| `void` | OnSprayLoop() |  | 
| `void` | OnSprayStart() |  | 
| `void` | OnSprayStop() |  | 
| `void` | SlowUpdateImbue() |  | 
| `void` | Throw(`Vector3` velocity) |  | 
| `void` | Unload() |  | 
| `void` | UpdateCaster() |  | 
| `void` | UpdateImbue(`Single` speedRatio) |  | 


## `SpellCastData`

```csharp
public class ThunderRoad.SpellCastData
    : SpellData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | aiCastMaxDistance |  | 
| `Single` | aiCastMinDistance |  | 
| `CastType` | aiCastType |  | 
| `Single` | loopMaxDuration |  | 
| `Single` | minMana |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `SpellCastData` | Clone() |  | 
| `void` | Fire(`Boolean` active) |  | 
| `void` | FireAxis(`Single` value) |  | 
| `void` | FixedUpdateCaster() |  | 
| `Int32` | GetCurrentVersion() |  | 
| `void` | Load(`SpellCaster` spellCaster, `Level` level) |  | 
| `void` | Unload() |  | 
| `void` | UpdateCaster() |  | 


## `SpellCaster`

```csharp
public class ThunderRoad.SpellCaster
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | allowCasting |  | 
| `Boolean` | allowSpellWheel |  | 
| `List<EffectInstance>` | fingerEffectInstances |  | 
| `Transform` | fire |  | 
| `Single` | fireAxis |  | 
| `Single` | fireTime |  | 
| `Boolean` | grabbedFire |  | 
| `List<ImbueObject>` | imbueObjects |  | 
| `Single` | imbueTransferMinIntensity |  | 
| `Trigger` | imbueTrigger |  | 
| `Single` | intensity |  | 
| `Boolean` | isFiring |  | 
| `Boolean` | isMerging |  | 
| `Boolean` | isSpraying |  | 
| `Transform` | magic |  | 
| `Single` | magicFollowSpeed |  | 
| `Vector3` | magicOffset |  | 
| `Transform` | magicSource |  | 
| `Mana` | mana |  | 
| `Single` | manaWaste |  | 
| `Single` | mergeAttractSpeed |  | 
| `SpellCaster` | other |  | 
| `Boolean` | parryable |  | 
| `RagdollHand` | ragdollHand |  | 
| `Transform` | rayDir |  | 
| `SpellCastData` | spellInstance |  | 
| `SpellTelekinesis` | telekinesis |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Fire(`Boolean` active) |  | 
| `void` | FireAxis(`Single` value) |  | 
| `Vector3` | GetShootDirection() |  | 
| `void` | LoadSpell(`SpellCastData` spellCastData, `Level` level) |  | 
| `void` | ManaFixedUpdate() |  | 
| `void` | ManaUpdate() |  | 
| `void` | OnHandGrab(`Side` side, `Handle` handle, `Single` axisPosition, `HandleOrientation` orientation, `EventTime` eventTime) |  | 
| `void` | OnHandUnGrab(`Side` side, `Handle` handle, `Boolean` throwing, `EventTime` eventTime) |  | 
| `void` | OnTriggerImbue(`Collider` other, `Boolean` enter) |  | 
| `void` | SetFingersEffect(`Single` intensity) |  | 
| `void` | SetMagicOffset(`Vector3` offset) |  | 
| `void` | SpawnFingersEffect(`EffectData` effectData, `Boolean` play = False, `Single` intensity = 1, `Transform` target = null) |  | 
| `void` | StopFingersEffect() |  | 
| `void` | UnloadSpell() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | throwMinHandVelocity |  | 


## `SpellCastGravity`

```csharp
public class ThunderRoad.SpellCastGravity
    : SpellCastCharge

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | halfSphereRadius |  | 
| `Single` | imbueAngularDrag |  | 
| `Single` | imbueDrag |  | 
| `Single` | imbueGravityFalloffThreshold |  | 
| `Single` | imbueGravityRatio |  | 
| `EffectData` | imbueHitEffectData |  | 
| `String` | imbueHitEffectId |  | 
| `Single` | imbueHitGravityRatio |  | 
| `Single` | imbueHitGroundConsumption |  | 
| `EffectData` | imbueHitGroundEffectData |  | 
| `String` | imbueHitGroundEffectId |  | 
| `Single` | imbueHitGroundExplosionUpwardModifier |  | 
| `ForceMode` | imbueHitGroundForceMode |  | 
| `Single` | imbueHitGroundLastTime |  | 
| `Single` | imbueHitGroundMaxForce |  | 
| `Single` | imbueHitGroundMaxRadius |  | 
| `Single` | imbueHitGroundMaxVelocity |  | 
| `Single` | imbueHitGroundMinForce |  | 
| `Single` | imbueHitGroundMinRadius |  | 
| `Single` | imbueHitGroundMinVelocity |  | 
| `Int32` | imbueHitGroundPushLevel |  | 
| `Single` | imbueHitGroundRechargeDelay |  | 
| `Single` | imbueHitGroundWaveSpeed |  | 
| `Single` | imbueHitGroundWaveUpdateRate |  | 
| `EffectData` | imbueHitItemEffectData |  | 
| `String` | imbueHitItemEffectId |  | 
| `Single` | imbueHitItemZeroGravityDuration |  | 
| `Single` | imbueHitMassRatio |  | 
| `EffectData` | imbueHitRagdollEffectData |  | 
| `String` | imbueHitRagdollEffectId |  | 
| `Single` | imbueHitRagdollZeroGravityDuration |  | 
| `Single` | imbueMassRatio |  | 
| `Single` | lastImbueFalloffAmount |  | 
| `Single` | minChargeToPushCreature |  | 
| `Single` | playerLocomotionDeactivate |  | 
| `Single` | pushExplosionUpwardModifier |  | 
| `ForceMode` | pushForceMode |  | 
| `Single` | pushForceOnPlayer |  | 
| `LayerMask` | pushLayerMask |  | 
| `Single` | pushMaxForce |  | 
| `Boolean` | pushUseExplosionForce |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `SpellCastGravity` | Clone() |  | 
| `void` | Fire(`Boolean` active) |  | 
| `void` | Load(`SpellCaster` spellCaster, `Level` level) |  | 
| `void` | Load(`Imbue` imbue, `Level` level) |  | 
| `void` | OnCatalogRefresh() |  | 
| `void` | OnImbueCollisionStart(`CollisionInstance` collisionInstance) |  | 
| `void` | Throw(`Vector3` velocity) |  | 
| `void` | Unload() |  | 
| `void` | UpdateImbue(`Single` speedRatio) |  | 


## `SpellCastLightning`

```csharp
public class ThunderRoad.SpellCastLightning
    : SpellCastCharge

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | boltDamage |  | 
| `EffectData` | boltEffectData |  | 
| `String` | boltEffectId |  | 
| `EffectInstance[]` | boltEffectInstances |  | 
| `Int32` | boltElectrocuteDuration |  | 
| `Single` | boltEnergyTransfer |  | 
| `Single` | boltHaptic |  | 
| `EffectData` | boltHitEffectData |  | 
| `String` | boltHitEffectId |  | 
| `EffectData` | boltHitImbueEffectData |  | 
| `String` | boltHitImbueEffectId |  | 
| `BoltHit[]` | boltHits |  | 
| `Int32` | boltIndex |  | 
| `EffectData` | boltLoopEffectData |  | 
| `String` | boltLoopEffectId |  | 
| `EffectInstance` | boltLoopEffectInstance |  | 
| `Single` | boltLoopFadoutDelay |  | 
| `Single` | boltMaxRange |  | 
| `BoltHit[]` | boltParryHits |  | 
| `Single` | boltPushForce |  | 
| `Transform[]` | boltTargets |  | 
| `Single` | coneAngle |  | 
| `Single` | fireDirectionAngle |  | 
| `Single` | headToFireMaxAngle |  | 
| `Single` | hitLookupMaxDiffRange |  | 
| `EffectData` | imbueHitEffectData |  | 
| `String` | imbueHitEffectId |  | 
| `EffectData` | imbueHitRagdollEffectData |  | 
| `String` | imbueHitRagdollEffectId |  | 
| `Vector2` | intervalMaxRange |  | 
| `Vector2` | intervalMinRange |  | 
| `Int32` | pushLevel |  | 
| `LayerMask` | rayMaskNpc |  | 
| `LayerMask` | rayMaskPlayer |  | 
| `Int32` | simultanousBolts |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `SpellCastLightning` | Clone() |  | 
| `void` | Fire(`Boolean` active) |  | 
| `void` | Hit(`ColliderGroup` colliderGroup, `Vector3` position, `Vector3` normal, `Vector3` velocity, `Single` intensity, `Boolean` forceElectrocute = False) |  | 
| `Int32` | HitLookup(`Single` coneAngle, `Single` radius) |  | 
| `void` | Load(`SpellCaster` spellCaster, `Level` level) |  | 
| `void` | OnCatalogRefresh() |  | 
| `void` | OnCrystalUse(`Side` side, `Boolean` active) |  | 
| `void` | OnImbueCollisionStart(`CollisionInstance` collisionInstance) |  | 
| `void` | OnSprayLoop() |  | 
| `void` | OnSprayStart() |  | 
| `void` | OnSprayStop() |  | 
| `BoltHit` | PickBoltHit(`Int32` count) |  | 
| `Single` | PickRangeFromForce(`Vector2` minRange, `Vector2` maxRange) |  | 
| `void` | Unload() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | boltHitsLenght |  | 


## `SpellCastProjectile`

```csharp
public class ThunderRoad.SpellCastProjectile
    : SpellCastCharge

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemMagicProjectile` | guidedProjectile |  | 
| `Single` | imbueUseConsumption |  | 
| `EffectData` | imbueUseEffectData |  | 
| `String` | imbueUseEffectId |  | 
| `Boolean` | projectileAllowDeflect |  | 
| `DamagerData` | projectileDamagerData |  | 
| `String` | projectileDamagerId |  | 
| `ItemData` | projectileData |  | 
| `EffectData` | projectileDefectEffectData |  | 
| `String` | projectileDeflectEffectId |  | 
| `EffectData` | projectileEffectData |  | 
| `String` | projectileEffectId |  | 
| `String` | projectileId |  | 
| `Single` | projectileImbueEnergyTransfered |  | 
| `Boolean` | projectilePlayerGuided |  | 
| `Single` | projectileVelocity |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `SpellCastProjectile` | Clone() |  | 
| `void` | Fire(`Boolean` active) |  | 
| `List<ValueDropdownItem<String>>` | GetAllDamagerID() |  | 
| `List<ValueDropdownItem<String>>` | GetAllItemID() |  | 
| `void` | OnCatalogRefresh() |  | 
| `void` | OnCrystalUse(`Side` side, `Boolean` active) |  | 
| `void` | OnProjectileCollision(`CollisionInstance` collisionInstance) |  | 
| `void` | OnProjectileDespawn(`EventTime` eventTime) |  | 
| `void` | StopProjectileGuidance() |  | 
| `void` | Throw(`Vector3` velocity) |  | 
| `void` | UpdateCaster() |  | 


## `SpellData`

```csharp
public class ThunderRoad.SpellData
    : CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Level` | level |  | 
| `Single` | manaConsumption |  | 
| `Single` | manaWaste |  | 


## `SpellMergeData`

```csharp
public class ThunderRoad.SpellMergeData
    : SpellData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `EffectInstance` | chargeEffect |  | 
| `EffectData` | chargeEffectData |  | 
| `String` | chargeEffectId |  | 
| `Single` | chargeSpeed |  | 
| `Single` | chargeStartHandsRatio |  | 
| `HandPoseData` | closeHandPoseData |  | 
| `String` | closeHandPoseId |  | 
| `Single` | currentCharge |  | 
| `EffectData` | fingerEffectData |  | 
| `String` | fingerEffectId |  | 
| `Single` | handCompletedDistance |  | 
| `Single` | handEnterAngle |  | 
| `Single` | handEnterDistance |  | 
| `Single` | handExitAngle |  | 
| `Single` | handExitDistance |  | 
| `String` | leftSpellId |  | 
| `Mana` | mana |  | 
| `HandPoseData` | openHandPoseData |  | 
| `String` | openHandPoseId |  | 
| `String` | rightSpellId |  | 
| `Boolean` | stopIfManaDepleted |  | 
| `Single` | stopSpeed |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CanMerge() |  | 
| `void` | FireAxis(`Single` value, `Side` side) |  | 
| `void` | FixedUpdate() |  | 
| `List<ValueDropdownItem<String>>` | GetAllEffectID() |  | 
| `List<ValueDropdownItem<String>>` | GetAllHandPoseID() |  | 
| `List<ValueDropdownItem<String>>` | GetAllSpellID() |  | 
| `Int32` | GetCurrentVersion() |  | 
| `void` | Load(`Mana` mana) |  | 
| `void` | Merge(`Boolean` active) |  | 
| `void` | OnCatalogRefresh() |  | 
| `void` | Unload() |  | 
| `void` | Update() |  | 


## `SpellMergeGravity`

```csharp
public class ThunderRoad.SpellMergeGravity
    : SpellMergeData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | bubbleActive |  | 
| `Single` | bubbleDuration |  | 
| `EffectData` | bubbleEffectData |  | 
| `String` | bubbleEffectId |  | 
| `Single` | bubbleEffectMaxScale |  | 
| `Single` | bubbleHandSeparationMaxAngle |  | 
| `Single` | bubbleMinCharge |  | 
| `AnimationCurve` | bubbleScaleCurveOverTime |  | 
| `Dictionary<Creature, HashSet<RagdollPart>>` | capturedCreatures |  | 
| `List<CollisionHandler>` | capturedObjects |  | 
| `Boolean` | capturedPlayer |  | 
| `Trigger` | captureTrigger |  | 
| `Boolean` | capturing |  | 
| `Single` | liftDrag |  | 
| `Single` | liftMaxForce |  | 
| `Single` | liftMinForce |  | 
| `Single` | liftRagdollForceMultiplier |  | 
| `Single` | mergingLiftRadius |  | 
| `Single` | playerGravityRatio |  | 
| `Vector3` | randomTorqueRange |  | 
| `Single` | throwDefaultForce |  | 
| `EffectData` | throwEffectData |  | 
| `String` | throwEffectId |  | 
| `Boolean` | throwEnabled |  | 
| `Single` | throwRagdollLimbForce |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `IEnumerator` | BubbleCoroutine(`Single` duration) |  | 
| `Boolean` | CanMerge() |  | 
| `void` | FireAxis(`Single` value, `Side` side) |  | 
| `void` | HandControl(`SpellCaster` spellCaster, `Boolean` active) |  | 
| `void` | Load(`Mana` mana) |  | 
| `void` | Merge(`Boolean` active) |  | 
| `void` | OnCatalogRefresh() |  | 
| `void` | OnTrigger(`Collider` other, `Boolean` enter) |  | 
| `void` | StartCapture(`Single` radius) |  | 
| `void` | StopCapture() |  | 
| `void` | Unload() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single[]` | randomHeightArray |  | 
| `Vector3[]` | randomTorqueArray |  | 


## `SpellPowerData`

```csharp
public class ThunderRoad.SpellPowerData
    : SpellData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Mana` | mana |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `SpellPowerData` | Clone() |  | 
| `List<ValueDropdownItem<String>>` | GetAllEffectID() |  | 
| `Int32` | GetCurrentVersion() |  | 
| `void` | Load(`Mana` mana) |  | 
| `void` | Unload() |  | 
| `void` | Update() |  | 
| `void` | Use() |  | 


## `SpellPowerSlowTime`

```csharp
public class ThunderRoad.SpellPowerSlowTime
    : SpellPowerData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `EffectData` | effectData |  | 
| `String` | effectId |  | 
| `AnimationCurve` | enterCurve |  | 
| `AnimationCurve` | exitCurve |  | 
| `Single` | focusConsumption |  | 
| `String` | focusDepletedEffectId |  | 
| `EffectData` | focusDepletedEffetData |  | 
| `Single` | focusMinToUse |  | 
| `Single` | scale |  | 
| `Boolean` | scaleToMixerParameter |  | 
| `String` | scaleToMixerParameterName |  | 
| `Boolean` | slowingTime |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `SpellPowerSlowTime` | Clone() |  | 
| `void` | Load(`Mana` mana) |  | 
| `void` | OnCatalogRefresh() |  | 
| `void` | Unload() |  | 
| `void` | Update() |  | 
| `void` | Use() |  | 


## `SpellTelekinesis`

```csharp
public class ThunderRoad.SpellTelekinesis
    : SpellData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | allowDismemberment |  | 
| `Single` | angularDrag |  | 
| `Boolean` | autoGrab |  | 
| `Handle` | catchedHandle |  | 
| `Single` | catchTime |  | 
| `HandPoseData` | closeHandPoseData |  | 
| `String` | closeHandPoseId |  | 
| `EffectInstance` | defaultHandEffect |  | 
| `EffectData` | defaultHandEffectData |  | 
| `String` | defaultHandEffectId |  | 
| `Single` | dismembermentBreakForceMultiplier |  | 
| `Single` | drag |  | 
| `AnimationCurve` | followDefaultSpeedCurve |  | 
| `AnimationCurve` | followRagdollSpeedCurve |  | 
| `Boolean` | grabRagdoll |  | 
| `Boolean` | gravity |  | 
| `Rigidbody` | grip |  | 
| `Single` | gripDistance |  | 
| `RaycastHit[]` | hits |  | 
| `ConfigurableJoint` | joint |  | 
| `Boolean` | justCatched |  | 
| `LayerMask` | layerMask |  | 
| `LayerMask` | lineOfSightMask |  | 
| `Single` | maxAngle |  | 
| `Single` | maxCatchDistance |  | 
| `Single` | maxVelocity |  | 
| `Single` | minFingersWeight |  | 
| `Single` | minVelocity |  | 
| `HandPoseData` | openHandPoseData |  | 
| `String` | openHandPoseId |  | 
| `Single` | positionDamper |  | 
| `Single` | positionMaxForce |  | 
| `Single` | positionSpring |  | 
| `Single` | pullAndRepelMaxSpeed |  | 
| `Single` | pullAndRepelNoDragThreshold |  | 
| `Single` | pullSpeed |  | 
| `Single` | pushDefaultForce |  | 
| `EffectData` | pushEffectData |  | 
| `String` | pushEffectId |  | 
| `Single` | pushRagdollForce |  | 
| `Single` | pushRagdollOtherPartsForce |  | 
| `Single` | radius |  | 
| `EffectInstance` | ragdollGripEffect |  | 
| `EffectData` | ragdollGripEffectData |  | 
| `String` | ragdollGripEffectId |  | 
| `EffectInstance` | ragdollHandEffect |  | 
| `EffectData` | ragdollHandEffectData |  | 
| `String` | ragdollHandEffectId |  | 
| `Single` | repelMaxDistance |  | 
| `Single` | repelSpeed |  | 
| `Single` | reverseAngle |  | 
| `Single` | rotationDamper |  | 
| `Single` | rotationMaxForce |  | 
| `Single` | rotationSpring |  | 
| `SpellCaster` | spellCaster |  | 
| `Boolean` | spinFromCenterOfMass |  | 
| `Boolean` | spinMode |  | 
| `Single` | spinStartTime |  | 
| `Boolean` | spinToogle |  | 
| `Single` | spinVelocity |  | 
| `AnimationCurve` | spinVelocityCurve |  | 
| `Handle` | targetHandle |  | 
| `Single` | throwMultiplier |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `SpellTelekinesis` | Clone() |  | 
| `void` | CreateJoint(`Handle` handle) |  | 
| `List<ValueDropdownItem<String>>` | GetAllEffectID() |  | 
| `List<ValueDropdownItem<String>>` | GetAllHandPoseID() |  | 
| `Vector2` | GetTelekinesisIntensity() |  | 
| `void` | Load(`SpellCaster` spellCaster) |  | 
| `void` | SetSpinMode(`Boolean` active) |  | 
| `void` | StartTargeting(`Handle` objectHandle) |  | 
| `void` | StopTargeting() |  | 
| `Boolean` | TryCatch() |  | 
| `Boolean` | TryRelease(`Boolean` tryThrow = False) |  | 
| `void` | Unload() |  | 
| `void` | Update() |  | 
| `void` | UpdateGrip() |  | 
| `void` | UpdateRayCast() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | holdGrip |  | 
| `Boolean` | showHighlighter |  | 


## `SphereCenterSolver`

```csharp
public class ThunderRoad.SphereCenterSolver

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3` | center |  | 
| `Single` | radius |  | 


## `SpringForceEffect`

```csharp
public class ThunderRoad.SpringForceEffect
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | active |  | 
| `Single` | connectedBodyMaxSpeed |  | 
| `Single` | connectedBodyMinSpeed |  | 
| `Single` | currentIntensity |  | 
| `String` | effectId |  | 
| `EffectInstance` | effectInstance |  | 
| `Single` | maxForce |  | 
| `Single` | minForce |  | 
| `SpringJoint` | springJoint |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | Update() |  | 


## `TestBallCollision`

```csharp
public class ThunderRoad.TestBallCollision
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `SphereCollider` | col |  | 
| `CollisionCallBack` | collisionCallBack |  | 
| `Rigidbody` | rb |  | 


## `TestEffect`

```csharp
public class ThunderRoad.TestEffect
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | collider |  | 
| `List<Effect>` | effects |  | 
| `Single` | intensity |  | 
| `Gradient` | mainGradient |  | 
| `Renderer` | mainRenderer |  | 
| `Mesh` | mesh |  | 
| `ParticleSystem` | rootParticleSystem |  | 
| `Gradient` | secondaryGradient |  | 
| `Renderer` | secondaryRenderer |  | 
| `Single` | speed |  | 
| `Transform` | target |  | 
| `Boolean` | useMainGradient |  | 
| `Boolean` | useSecondaryGradient |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnValidate() |  | 
| `void` | Play() |  | 
| `void` | Refresh() |  | 
| `void` | Stop() |  | 
| `void` | TestIntensity(`Single` duration) |  | 


## `TestEffectManager`

```csharp
public class ThunderRoad.TestEffectManager
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<EffectCollection>` | effects |  | 


## `TestRaycast`

```csharp
public class ThunderRoad.TestRaycast
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector2` | angles |  | 
| `Foot` | footLeft |  | 
| `Foot` | footRight |  | 
| `Vector3` | footSize |  | 
| `Boolean` | showDebug |  | 
| `Int32` | sphereCastHitCount |  | 
| `RaycastHit[]` | sphereCastHits |  | 
| `LayerMask` | sphereCastLayerMask |  | 
| `Single` | sphereCastRadius |  | 
| `Single` | stepAngle |  | 
| `Single` | sweepDistance |  | 
| `Single` | sweepMaxHorizontalAngle |  | 
| `Single` | sweepMaxVerticalAngle |  | 
| `Single` | sweepRate |  | 
| `Transform` | target |  | 
| `Single` | upMaxAngle |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | CastSweep() |  | 
| `void` | OnDrawGizmos() |  | 
| `void` | Refresh() |  | 
| `Boolean` | SphereCastAngle(`Single` verticalAngle, `Single` horizontalAngle, `RaycastHit&` hitInfo) |  | 
| `void` | SphereCastVertical(`Single` horizontalAngle) |  | 


## `TestRayUv`

```csharp
public class ThunderRoad.TestRayUv
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Material` | material |  | 
| `Int32` | materialIndex |  | 
| `Mesh` | mesh |  | 
| `String` | propertyID |  | 
| `TestBallCollision` | testBallCollisionPrefab |  | 
| `Texture2D` | tex2D |  | 
| `Vector2` | textureCoord |  | 
| `Vector2` | textureCoord2 |  | 
| `Single` | throwForce |  | 
| `Color` | uvColor |  | 
| `Color` | uvColor2 |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | GetUv(`RagdollPart` ragdollPart, `Vector3` position, `Vector3` direction) |  | 
| `void` | GetUv(`Mesh` mesh, `SkinnedMeshRenderer` skinnedMeshRenderer, `RaycastHit&` raycastHit) |  | 
| `void` | ThrowBall() |  | 


## `TextData`

```csharp
public class ThunderRoad.TextData
    : CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Item>` | items |  | 
| `List<PageGroup>` | pageGroups |  | 
| `List<TextID>` | strings |  | 
| `List<TextGroup>` | textGroups |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | GetCurrentVersion() |  | 
| `List<ValueDropdownItem<String>>` | GetDropdownAllTextGroups() |  | 
| `List<ValueDropdownItem<String>>` | GetDropdownAllTexts(`String` groupId) |  | 
| `TextGroup` | GetGroup(`String` groupId) |  | 
| `PageGroup` | GetPageGroup(`String` id) |  | 
| `String` | GetString(`String` groupId, `String` id) |  | 
| `IEnumerator` | OnCatalogRefreshCoroutine() |  | 


## `ThirdPersonView`

```csharp
public class ThunderRoad.ThirdPersonView
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Camera` | cam |  | 
| `UniversalAdditionalCameraData` | cameraData |  | 
| `Boolean` | isActive |  | 
| `Single` | moveSpeed |  | 
| `Player` | player |  | 
| `Single` | snapTurnDelay |  | 
| `TrackedPoseDriver` | trackedPoseDriver |  | 
| `Single` | turnSpeed |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Activate(`Boolean` active) |  | 
| `void` | AutoPosition() |  | 
| `void` | Move(`Vector3` direction) |  | 
| `void` | Toogle() |  | 
| `void` | Turn(`Single` speed) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `ThirdPersonView` | local |  | 
| `TurnMode` | turnMode |  | 


Static Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `ToggleEvent` | onToggle |  | 


## `Trigger`

```csharp
public class ThunderRoad.Trigger
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | active |  | 
| `CallBack` | callBack |  | 
| `SphereCollider` | sphereCollider |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | OnTriggerEnter(`Collider` other) |  | 
| `void` | OnTriggerExit(`Collider` other) |  | 
| `void` | SetActive(`Boolean` active) |  | 
| `void` | SetCallback(`CallBack` callback) |  | 
| `void` | SetLayer(`Int32` layer) |  | 
| `void` | SetRadius(`Single` radius) |  | 


## `Tube`

```csharp
public class ThunderRoad.Tube
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Color` | color |  | 
| `Boolean` | loadOnStart |  | 
| `Vector3` | nodeAngle |  | 
| `String` | shaderName |  | 
| `Single` | sphereScale |  | 
| `Texture2D` | sphereTexture |  | 
| `tubeJointType` | srcJointType |  | 
| `Transform` | srcNode |  | 
| `tubeJointType` | tgtJointType |  | 
| `Transform` | tgtNode |  | 
| `Texture2D` | tubeJoinedTexture |  | 
| `Single` | tubeScale |  | 
| `Single` | tubeTexTilingOffset |  | 
| `Texture2D` | tubeTexture |  | 
| `Boolean` | updateContinually |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DisableCollision(`Boolean` active) |  | 
| `void` | Load() |  | 
| `void` | SetColor(`Color` colorToSet) |  | 
| `void` | SetShader(`String` shaderName) |  | 
| `void` | SetSphereScale(`Single` scale) |  | 
| `void` | SetTexture(`Texture2D` textureToSet) |  | 
| `void` | SetTubeScale(`Single` scale) |  | 
| `void` | SetTubeSphereScale(`Single` scale) |  | 
| `void` | UnLoad() |  | 


## `TubeBuilder`

```csharp
public class ThunderRoad.TubeBuilder
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | continuousUpdate |  | 
| `Int32` | layer |  | 
| `Material` | material |  | 
| `PhysicMaterial` | physicMaterial |  | 
| `Boolean` | preGenerate |  | 
| `Single` | radius |  | 
| `Transform` | target |  | 
| `Single` | tilingOffset |  | 
| `MeshRenderer` | tube |  | 
| `Boolean` | useCollider |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | ClearTube() |  | 
| `void` | Generate() |  | 
| `void` | OnDrawGizmos() |  | 
| `void` | OnValidate() |  | 
| `void` | Update() |  | 
| `void` | UpdateTube() |  | 


## `TurnMapSelectionSphere`

```csharp
public class ThunderRoad.TurnMapSelectionSphere
    : MonoBehaviour

```

## `TutorialData`

```csharp
public class ThunderRoad.TutorialData
    : CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Step>` | steps |  | 
| `Single` | textFollowCamSpeed |  | 


## `TypeExtensions`

```csharp
public static class ThunderRoad.TypeExtensions

```

Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | GetListType(this `Type` type) |  | 


## `UIButton`

```csharp
public class ThunderRoad.UIButton
    : MonoBehaviour, IPointerClickHandler, IEventSystemHandler

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Selectable` | selectable |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | OnButtonPressed() |  | 
| `void` | OnPointerClick(`PointerEventData` eventData) |  | 


## `UIButtonLink`

```csharp
public class ThunderRoad.UIButtonLink
    : UIButton, IPointerClickHandler, IEventSystemHandler

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | httpLink |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnButtonPressed() |  | 


## `UIButtonLoadLevel`

```csharp
public class ThunderRoad.UIButtonLoadLevel
    : UIButton, IPointerClickHandler, IEventSystemHandler

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | disableIfAlreadyLoaded |  | 
| `String` | levelName |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnButtonPressed() |  | 


## `UIButtonMisc`

```csharp
public class ThunderRoad.UIButtonMisc
    : UIButton, IPointerClickHandler, IEventSystemHandler

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Action` | action |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnButtonPressed() |  | 


## `UIButtonOpenFolder`

```csharp
public class ThunderRoad.UIButtonOpenFolder
    : UIButton, IPointerClickHandler, IEventSystemHandler

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Folder` | folder |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnButtonPressed() |  | 


## `UIDropdownLevel`

```csharp
public class ThunderRoad.UIDropdownLevel
    : MonoBehaviour

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Refresh() |  | 


## `UIInputSelector`

```csharp
public class ThunderRoad.UIInputSelector
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | cosmosPage |  | 
| `Int32` | forcePage |  | 
| `GameObject` | indexPage |  | 
| `GameObject` | oculusPage |  | 
| `GameObject` | oculusSteamVRPage |  | 
| `GameObject` | VivePage |  | 
| `GameObject` | wmr2Page |  | 
| `GameObject` | wmrPage |  | 


## `UIItemSpawner`

```csharp
public class ThunderRoad.UIItemSpawner
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Texture>` | addressableCategoryTextures |  | 
| `List<Texture>` | addressableItemTextures |  | 
| `GridLayoutGroup` | categoriesLayout |  | 
| `GameObject` | categoriesPage |  | 
| `Container` | container |  | 
| `GameObject` | iconPrefab |  | 
| `GameObject` | itemPreviewPage |  | 
| `GridLayoutGroup` | itemsLayout |  | 
| `GameObject` | itemsPage |  | 
| `GameObject` | itemStatsPage |  | 
| `Queue<Item>` | lastItemsSpawned |  | 
| `Content` | selectedContent |  | 
| `DamagerData` | selectedDamager |  | 
| `Boolean` | showExistingOnly |  | 
| `Button` | spawnButton |  | 
| `Transform` | spawnPoint |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | GrabSelectedItem() |  | 
| `void` | OnContentLoadedEvent() |  | 
| `void` | OnDrawGizmos() |  | 
| `void` | RefreshCategories() |  | 
| `void` | RefreshItems(`Container` container, `String` storageCategoryFilter = null) |  | 
| `void` | SetCategory(`GameObject` target, `Category` iconData) |  | 
| `void` | SetItem(`GameObject` target, `Content` content) |  | 
| `void` | SetPageItemDetail() |  | 
| `void` | SetPageItemList() |  | 
| `void` | SetSpawnButtonToEnabled() |  | 
| `void` | SpawnSelectedItem() |  | 


## `UIList`

```csharp
public class ThunderRoad.UIList
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Button` | btnNext |  | 
| `Button` | btnPrevious |  | 
| `Int32` | index |  | 
| `ToggleEvent` | onToggleEvent |  | 
| `Text` | value |  | 
| `List<Bool>` | valuesBool |  | 
| `List<CatalogItem>` | valuesCatalogItem |  | 
| `List<Float>` | valuesFloat |  | 
| `List<Int>` | valuesInt |  | 
| `List<String>` | valuesString |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddValue(`String` title, `Boolean` value) |  | 
| `void` | AddValue(`String` title, `Single` value) |  | 
| `void` | AddValue(`String` title, `Int32` value) |  | 
| `void` | AddValue(`String` title, `CatalogData` value) |  | 
| `void` | AddValue(`String` title, `String` value) |  | 
| `void` | Awake() |  | 
| `Boolean` | GetCurrentValueBool() |  | 
| `CatalogData` | GetCurrentValueCatalogData() |  | 
| `Single` | GetCurrentValueFloat() |  | 
| `Int32` | GetCurrentValueInt() |  | 
| `String` | GetCurrentValueString() |  | 
| `Int32` | GetIndex(`Boolean` value) |  | 
| `Int32` | GetIndex(`Single` value) |  | 
| `Int32` | GetIndex(`Int32` value) |  | 
| `Int32` | GetIndex(`CatalogData` value) |  | 
| `Int32` | GetIndex(`String` value) |  | 
| `void` | InitValues() |  | 
| `void` | LoadValue() |  | 
| `void` | NextValue() |  | 
| `void` | OnEnable() |  | 
| `void` | OnIndexChanged() |  | 
| `void` | OnValidate() |  | 
| `void` | PreviousValue() |  | 
| `void` | RefreshDisplay() |  | 
| `void` | SetInteractable(`Boolean` active) |  | 
| `void` | Start() |  | 


## `UIListDebug`

```csharp
public class ThunderRoad.UIListDebug
    : UIList

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Parameter` | parameter |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | InitValues() |  | 
| `void` | LoadValue() |  | 
| `void` | OnIndexChanged() |  | 
| `void` | RefreshDisplay() |  | 


## `UIListLevelMode`

```csharp
public class ThunderRoad.UIListLevelMode
    : UIList

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddValueAndDesc(`String` aModeName, `String` aDesc) |  | 
| `void` | ClearValues() |  | 
| `String` | GetValue() |  | 
| `void` | InitValues() |  | 
| `void` | OnIndexChanged() |  | 


## `UIListOptions`

```csharp
public class ThunderRoad.UIListOptions
    : UIList

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Option` | option |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | InitValues() |  | 
| `void` | LoadValue() |  | 
| `void` | OnIndexChanged() |  | 


## `UIMap`

```csharp
public class ThunderRoad.UIMap
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<LevelData>` | allLevelDatas |  | 
| `List<Button>` | allLocations |  | 
| `Button` | bulletPointPrefab |  | 
| `Transform` | canvasDetails |  | 
| `Int32` | currentGameModIndex |  | 
| `Int32` | currentIndexOption |  | 
| `List<LevelData>` | currentLevelDatas |  | 
| `GameObject` | currentMap |  | 
| `List<Option>` | currentOptions |  | 
| `Int32` | currentPage |  | 
| `Text` | descriptionText |  | 
| `Text` | gameModTitle |  | 
| `UIMapBulletPoint` | lastSelected |  | 
| `LevelData` | levelData |  | 
| `UISelectionListButtonsLevelModeOption` | LevelModeOptionPrefab |  | 
| `List<UISelectionListButtonsLevelModeOption>` | levelModeOptions |  | 
| `List<Texture2D>` | loadedTextures |  | 
| `Transform` | locationRoot |  | 
| `List<Transform>` | locations |  | 
| `String` | mapId |  | 
| `Transform` | mapParent |  | 
| `MeshRenderer` | mapRenderer |  | 
| `RawImage` | mapSketch |  | 
| `Text` | mapTitleText |  | 
| `Int32` | maxPage |  | 
| `Text` | modeDescriptionText |  | 
| `Int32` | modeIndex |  | 
| `List<String>` | mods |  | 
| `List<GameObject>` | modsMapObject |  | 
| `List<Texture2D>` | modsMapTextures |  | 
| `Button` | nextOptionsButton |  | 
| `Single` | optionSpacingSize |  | 
| `Transform` | optionsPanel |  | 
| `ToggleGroup` | orbGroup |  | 
| `Text` | pageText |  | 
| `Button` | previousOptionsButton |  | 
| `Int32` | startIndexOption |  | 
| `Button` | travelButton |  | 
| `UIMapLevelMode` | uiLevelSelectorLevelMode |  | 
| `List<Transform>` | usedLocations |  | 
| `Single` | visibleRadius |  | 
| `Transform` | wholeMap |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | CreateLocationNew(`Transform` location, `LevelData` levelData) |  | 
| `IEnumerator` | InitCoroutine() |  | 
| `void` | NextGameMod() |  | 
| `void` | NextMode() |  | 
| `void` | NextOptions() |  | 
| `void` | OnDrawGizmos() |  | 
| `void` | PreviousGameMod() |  | 
| `void` | PreviousMode() |  | 
| `void` | PreviousOptions() |  | 
| `void` | SetNextLocation() |  | 
| `void` | SetPageNone() |  | 
| `void` | SetPageSelected(`LevelData` levelData) |  | 
| `void` | SetPreviousLocation() |  | 


## `UIMapLevelMode`

```csharp
public class ThunderRoad.UIMapLevelMode
    : UISelectionListButtons

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Text` | levelModeDescription |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `String` | GetCurrentLevelMode() |  | 
| `void` | OnUpdateValue() |  | 
| `void` | RefreshDisplay() |  | 
| `void` | UpdateValues(`LevelData` levelData) |  | 


## `UIRoomTester`

```csharp
public class ThunderRoad.UIRoomTester
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `DungeonFlow` | dungeonFlow |  | 
| `String` | dungeonFlowAddress |  | 
| `Int32` | i |  | 
| `GameObject` | roomLinePrefab |  | 
| `GameObject` | selectedRoom |  | 
| `Button` | startButton |  | 
| `Transform` | startSpawn |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Start() |  | 


## `UISelectionListButtons`

```csharp
public class ThunderRoad.UISelectionListButtons
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `CharacterSelection` | characterSelectionNew |  | 
| `RawImage` | colorViewer |  | 
| `RawImage` | colorViewer2 |  | 
| `Int32` | currentValue |  | 
| `Boolean` | isInteractable |  | 
| `Int32` | maxValue |  | 
| `Int32` | minValue |  | 
| `Button` | nextButton |  | 
| `Button` | previousButton |  | 
| `Text` | title |  | 
| `Text` | value |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `Int32` | GetCurrentValue() |  | 
| `void` | LoadValue() |  | 
| `void` | NextValue() |  | 
| `void` | OnUpdateValue() |  | 
| `void` | OnValidate() |  | 
| `void` | PreviousValue() |  | 
| `void` | Refresh() |  | 
| `void` | RefreshDisplay() |  | 
| `void` | SetInteractable(`Boolean` active) |  | 


## `UISelectionListButtonsBool`

```csharp
public class ThunderRoad.UISelectionListButtonsBool
    : UISelectionListButtons

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `Boolean` | GetCurrentBoolValue() |  | 
| `void` | LoadValue() |  | 
| `void` | OnUpdateValue() |  | 
| `void` | RefreshDisplay() |  | 


## `UISelectionListButtonsColor`

```csharp
public class ThunderRoad.UISelectionListButtonsColor
    : UISelectionListButtons

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Color>` | availableColors |  | 
| `List<EyeColor>` | availableEyesColors |  | 
| `List<HairColor>` | availableHairColors |  | 
| `PartColor` | color |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | LoadValue() |  | 
| `void` | OnUpdateValue() |  | 
| `void` | RefreshDisplay() |  | 


## `UISelectionListButtonsGameMode`

```csharp
public class ThunderRoad.UISelectionListButtonsGameMode
    : UISelectionListButtons

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<GameMode>` | availableGameModes |  | 
| `Text` | gameModeDescription |  | 
| `RawImage` | gameModeImage |  | 
| `Text` | gameModeWarning |  | 
| `Button` | selectButton |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `GameMode` | GetCurrentGameMode() |  | 
| `void` | LoadValue() |  | 
| `void` | OnUpdateValue() |  | 
| `void` | RefreshDisplay() |  | 


## `UISelectionListButtonsHeight`

```csharp
public class ThunderRoad.UISelectionListButtonsHeight
    : UISelectionListButtons

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | LoadValue() |  | 
| `void` | OnUpdateValue() |  | 
| `void` | RefreshDisplay() |  | 
| `void` | SetCurrentValue(`Single` height) |  | 


## `UISelectionListButtonsHeightImperial`

```csharp
public class ThunderRoad.UISelectionListButtonsHeightImperial
    : UISelectionListButtons

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `ImperialType` | imperialType |  | 
| `UISelectionListButtonsHeightImperial` | otherHeightSection |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | LoadValue() |  | 
| `void` | OnUpdateValue() |  | 
| `void` | RefreshDisplay() |  | 
| `void` | SetCurrentValue(`Single` height) |  | 


## `UISelectionListButtonsLevelModeOption`

```csharp
public class ThunderRoad.UISelectionListButtonsLevelModeOption
    : UISelectionListButtons, IPointerEnterHandler, IEventSystemHandler, IPointerExitHandler

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Option` | currentOption |  | 
| `String` | descriptionText |  | 
| `Type` | optionType |  | 
| `Sprite` | starImage |  | 
| `Sprite` | starImageFill |  | 
| `Image` | starImagePrefab |  | 
| `Transform` | starPlace |  | 
| `String` | textGroupId |  | 
| `UISelectionListButtonsBool` | toggle |  | 
| `UIMap` | uiLevelSelector |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | FullInit() |  | 
| `List<ValueDropdownItem<String>>` | GetAllTextGroupID() |  | 
| `Int32` | GetValue() |  | 
| `void` | InitValues() |  | 
| `void` | LoadValue() |  | 
| `void` | OnPointerEnter(`PointerEventData` eventData) |  | 
| `void` | OnPointerExit(`PointerEventData` eventData) |  | 
| `void` | OnUpdateValue() |  | 
| `void` | RefreshDisplay() |  | 


## `UISelectionListButtonsMapSelection`

```csharp
public class ThunderRoad.UISelectionListButtonsMapSelection
    : UISelectionListButtons

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Text` | levelCount |  | 
| `Text` | levelDescription |  | 
| `RawImage` | levelImage |  | 
| `UIMapLevelMode` | UISelectionLevelMode |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `LevelData` | GetCurrentLevel() |  | 
| `void` | LoadValue() |  | 
| `void` | OnUpdateValue() |  | 
| `void` | RefreshDisplay() |  | 


## `UISelectionListButtonsSwitchMeterImperial`

```csharp
public class ThunderRoad.UISelectionListButtonsSwitchMeterImperial
    : UISelectionListButtons

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `UISelectionListButtonsHeightImperial` | imperialFeetInput |  | 
| `UISelectionListButtonsHeightImperial` | imperialInchInput |  | 
| `UISelectionListButtonsHeight` | meterInput |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | OnUpdateValue() |  | 
| `void` | RefreshDisplay() |  | 


## `UISelectionListButtonsWardrobe`

```csharp
public class ThunderRoad.UISelectionListButtonsWardrobe
    : UISelectionListButtons

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | allowNothing |  | 
| `WardRobeCategory` | category |  | 
| `String` | channel |  | 
| `String` | layer |  | 
| `List<ItemModuleWardrobe>` | wardrobes |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnUpdateValue() |  | 
| `void` | OnValidate() |  | 
| `void` | Refresh() |  | 


## `UISetTextValue`

```csharp
public class ThunderRoad.UISetTextValue
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | text |  | 
| `Text` | textComponent |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | SetValue(`Single` value) |  | 


## `UIText`

```csharp
public class ThunderRoad.UIText
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | forceUpperCase |  | 
| `String` | text |  | 
| `Text` | textComponent |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | OnEnable() |  | 
| `void` | Refresh() |  | 


## `UITextInventory`

```csharp
public class ThunderRoad.UITextInventory
    : UIText

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `UIItemSpawner` | inventory |  | 
| `Value` | value |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | Refresh() |  | 


## `UITextMisc`

```csharp
public class ThunderRoad.UITextMisc
    : UIText

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Value` | value |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Refresh() |  | 


## `UITextScores`

```csharp
public class ThunderRoad.UITextScores
    : UIText

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `LevelModuleXP` | levelModuleXP |  | 
| `Value` | value |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | Refresh() |  | 


## `UIVRStats`

```csharp
public class ThunderRoad.UIVRStats
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | droppedFrameCountAlertThreshold |  | 
| `Text` | droppedFrameCountText |  | 
| `Single` | droppedFrameCountWarningThreshold |  | 
| `Boolean` | dynamicColor |  | 
| `Text` | fpsText |  | 
| `Text` | framePresentCountText |  | 
| `Single` | GPUTimeLastFrameAlertThreshold |  | 
| `Text` | GPUTimeLastFrameText |  | 
| `Single` | GPUTimeLastFrameWarningThreshold |  | 


## `UIWaveSpawner`

```csharp
public class ThunderRoad.UIWaveSpawner
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | categoryPrefab |  | 
| `Text` | descriptionText |  | 
| `Int32` | difficulty |  | 
| `Text` | healthModifierText |  | 
| `String` | id |  | 
| `Text` | npcCountText |  | 
| `GameObject` | progressPageLeft |  | 
| `GameObject` | progressPageRight |  | 
| `Button` | startButton |  | 
| `Single` | startDelay |  | 
| `Text` | stateText |  | 
| `Button` | stopButton |  | 
| `Text` | stopButtonText |  | 
| `Text` | titleText |  | 
| `WaveData` | waveData |  | 
| `GameObject` | wavePageLeft |  | 
| `GameObject` | wavePageRight |  | 
| `GameObject` | wavePrefab |  | 
| `WaveSpawner` | waveSpawner |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | OnDestroy() |  | 
| `void` | OnDrawGizmos() |  | 
| `void` | OnWaveEnded() |  | 
| `void` | OnWaveStarted() |  | 


## `Utils`

```csharp
public static class ThunderRoad.Utils

```

Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | AddSpacesToSentence(`String` text, `Boolean` preserveAcronyms) |  | 
| `Single` | CalculateRatio(`Single` input, `Single` inputMin, `Single` inputMax, `Single` outputMin, `Single` outputMax) |  | 
| `Vector3` | ClampMagnitude(`Vector3` v, `Single` max, `Single` min) |  | 
| `CharacterJoint` | CloneCharacterJoint(`CharacterJoint` source, `GameObject` destination, `Rigidbody` newRigidbody = null) |  | 
| `Vector3` | ClosestDirection(`Vector3` direction, `Cardinal` cardinal) |  | 
| `Vector3` | ClosestPointOnLine(`Vector3` lineStart, `Vector3` lineEnd, `Vector3` point) |  | 
| `Vector3` | ClosestPointOnSurface(`Collider` collider, `Vector3` point, `Boolean&` isInside) |  | 
| `void` | ClosestPointOnSurface(`Collider` collider, `Vector3` lineStart, `Vector3` lineStop, `Vector3&` colliderPoint, `Vector3&` linePoint, `Boolean&` isInside) |  | 
| `Boolean` | ClosestPointsOnTwoLines(`Vector3` lineStart1, `Vector3` lineEnd1, `Vector3` lineStart2, `Vector3` lineEnd2, `Vector3&` closestPointLine1, `Vector3&` closestPointLine2) |  | 
| `Color` | ColorFromHSV(`Double` hue, `Double` saturation, `Double` value) |  | 
| `Component` | CopyComponent(`Component` original, `GameObject` destination) |  | 
| `void` | CopyComponentFieldsValues(`Component` sourceComponent, `Component` destinationComponent, `Boolean` publicOnly, `Boolean` readOnlyAttribute) |  | 
| `IEnumerator` | FadeIn(`AudioSource` audioSource, `Single` FadeTime) |  | 
| `IEnumerator` | FadeOut(`AudioSource` audioSource, `Single` FadeTime) |  | 
| `Color` | FromArgb(`Int32` alpha, `Int32` red, `Int32` green, `Int32` blue) |  | 
| `Vector2` | GetAngles(`Transform` reference, `Vector3` targetPosition) |  | 
| `Single` | GetAxisAngle(`Vector2` axis) |  | 
| `AxisDirection` | GetAxisDirection(`Vector2` axis, `Single` deadzone = 0) |  | 
| `Component` | GetClosest(`Vector3` position, `Component[]` others) |  | 
| `Collider` | GetClosest(`Vector3` position, `Collider[]` others, `Vector3&` closestColliderPoint, `Int32` arrayLenght = 0) |  | 
| `MonoBehaviour` | GetClosest(`Transform` source, `MonoBehaviour[]` others) |  | 
| `MonoBehaviour` | GetClosest(`Vector3` sourcePos, `MonoBehaviour[]` others) |  | 
| `List<Transform>` | GetClosestList(`Transform` source, `List<Transform>` others) |  | 
| `Dictionary<FieldInfo, Object>` | GetComponentFieldsValues(`Component` component) |  | 
| `LayerMask` | GetLayer(`LayerType` layerType) |  | 
| `Vector3` | GetLinearVelocityAtPoint(`Rigidbody` rigidbody, `Vector3` position, `Vector3` velocity, `Vector3` angularVelocity) |  | 
| `String` | GetTransformPath(`Transform` root, `Transform` transform) |  | 
| `void` | IgnoreLayerCollision(`Int32` layer, `LayerMask` layerMask) |  | 
| `Boolean` | InsideCollider(`Collider` collider, `Vector3` point) |  | 
| `Vector3` | InverseTransformPointUnscaled(this `Transform` transform, `Vector3` position) |  | 
| `Quaternion` | LookRotation(`Vector3` direction, `Vector3` localDirection, `Vector3` upward) |  | 
| `void` | MoveToFrontHead(`Transform` transf, `Transform` head, `Single` distance, `Transform` finger = null) |  | 
| `Single` | PercentageBetween(`Single` start, `Single` current, `Single` end) |  | 
| `Color` | Rainbow(`Single` progress) |  | 
| `Single` | RoundDownToNearest(`Single` value, `Single` roundto) |  | 
| `Vector3` | RoundVector3(`Vector3` vector3, `Int32` dp = 10) |  | 
| `void` | SetAndApplyGamma(this `Texture2D` tex, `Single` gamma = 2.2) |  | 
| `void` | SetComponentFieldsValues(`Component` component, `Dictionary<FieldInfo, Object>` fieldsValues) |  | 
| `void` | SetPositiveLocalScale(`Transform` transform) |  | 
| `String` | ToDetailedString(this `Vector3` v) |  | 
| `Vector3` | TransformPointUnscaled(this `Transform` transform, `Vector3` position) |  | 


## `VoiceData`

```csharp
public class ThunderRoad.VoiceData
    : CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Dialog>` | dialogs |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Load() |  | 
| `Boolean` | TryGetDialog(`Int32` dialogHashId, `Dialog&` dialog) |  | 
| `void` | Unload() |  | 


## `WaveData`

```csharp
public class ThunderRoad.WaveData
    : CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | alwaysAvailable |  | 
| `String` | category |  | 
| `String` | description |  | 
| `Single` | enemiesHealthMultiplier |  | 
| `List<Group>` | groups |  | 
| `Boolean` | loop |  | 
| `Int32` | maxAlive |  | 
| `Single` | maxTotalCount |  | 
| `Single` | minTotalCount |  | 
| `Single` | playerHealthMultiplier |  | 
| `String` | title |  | 
| `List<String>` | waveSelectors |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `CatalogData` | Clone() |  | 
| `Int32` | GetCurrentVersion() |  | 
| `Int32` | GetMaxAlive() |  | 
| `void` | OnCatalogRefresh() |  | 


## `WaveSpawner`

```csharp
public class ThunderRoad.WaveSpawner
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | addAsFleepointOnStart |  | 
| `Int32` | aliveCount |  | 
| `AudioContainer` | audioGroupWave |  | 
| `AudioSource` | audioMusic |  | 
| `AudioSource` | audioStep |  | 
| `SpawnPoint[]` | availableSpawnPoints |  | 
| `Boolean` | beginWaveOnStart |  | 
| `Single` | beginWaveOnStartDelay |  | 
| `Boolean` | cleanBodiesAndItemsOnWaveStart |  | 
| `Single` | delayedStartTimeLeft |  | 
| `Boolean` | groupCoroutineRunning |  | 
| `Int32` | ignoredFactionId |  | 
| `Boolean` | isRunning |  | 
| `Single` | musicAudioVolume |  | 
| `String` | musicWaveAddress |  | 
| `UnityEvent` | OnWaveBeginEvent |  | 
| `UnityEvent` | OnWaveEndEvent |  | 
| `UnityEvent` | OnWaveLoopEvent |  | 
| `Boolean` | pooled |  | 
| `Room` | room |  | 
| `Single` | sameSpawnDelay |  | 
| `Single` | spawnDelay |  | 
| `List<SpawnGroup>` | spawnGroups |  | 
| `List<SpawnPoint>` | spawnPoints |  | 
| `List<Transform>` | spawns |  | 
| `Coroutine` | startGroupCoroutine |  | 
| `Coroutine` | startWaveCoroutine |  | 
| `String` | startWaveId |  | 
| `String` | stepAudioGroupAddress |  | 
| `Single` | stepAudioVolume |  | 
| `Coroutine` | updateCoroutine |  | 
| `Single` | updateRate |  | 
| `Int32` | waveCount |  | 
| `WaveData` | waveData |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CancelWave() |  | 
| `void` | Clean() |  | 
| `List<ValueDropdownItem<Int32>>` | GetAllFactionID() |  | 
| `List<ValueDropdownItem<String>>` | GetAllWaveID() |  | 
| `void` | OnDisable() |  | 
| `SpawnPoint` | PickSpawnPoint(`Int32` index = -1) |  | 
| `void` | SetHealthMultiplier(`Creature` creature, `Single` multiplier) |  | 
| `void` | StartSpawnGroup(`SpawnGroup` spawnGroup) |  | 
| `void` | StartWave(`String` waveId) |  | 
| `void` | StartWave(`String` waveId, `Single` delay = 0, `Boolean` resetWaveCount = True) |  | 
| `void` | StartWave(`WaveData` waveData, `Single` delay = 0, `Boolean` resetWaveCount = True) |  | 
| `IEnumerator` | StartWaveCoroutine(`Single` delay) |  | 
| `void` | StopWave(`Boolean` success) |  | 
| `IEnumerator` | UpdateSpawner() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<WaveSpawner>` | instances |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | TryGetRunningInstance(`WaveSpawner&` waveSpawner) |  | 


## `WayPoint`

```csharp
public class ThunderRoad.WayPoint
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AnimationData` | animationData |  | 
| `String` | animationId |  | 
| `Vector2` | animationRandomMinMaxDelay |  | 
| `Single` | animationTurnMinAngle |  | 
| `Boolean` | playAnimation |  | 
| `Single` | turnSpeedRatio |  | 
| `Boolean` | turnToDirection |  | 
| `Vector2` | waitMinMaxDuration |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<ValueDropdownItem<String>>` | GetAllAnimationID() |  | 
| `void` | OnDrawGizmos() |  | 
| `void` | OnDrawGizmosSelected() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `NavMeshPath` | navMeshPath |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | SpawnerDrawGizmos(`Transform` spawner, `Transform` waypoints) |  | 


## `WeaponRack`

```csharp
public class ThunderRoad.WeaponRack
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Holder>` | holders |  | 
| `Boolean` | playerRack |  | 
| `String` | rackId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | LoadFromPlayerData() |  | 
| `void` | OnSnap(`Item` item) |  | 
| `void` | OnUnSnap(`Item` item) |  | 
| `void` | SaveToPlayerData() |  | 


## `Wearable`

```csharp
public class ThunderRoad.Wearable
    : Interactable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioContainer` | audioContainer |  | 
| `Creature` | creature |  | 
| `Side` | hudSide |  | 
| `String` | wardrobeChannel |  | 
| `String[]` | wardrobeLayers |  | 
| `Int32[]` | wardrobeLayersInt |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `Boolean` | CanTouch(`RagdollHand` ragdollHand) |  | 
| `InteractionResult` | CheckInteraction(`RagdollHand` ragdollHand) |  | 
| `void` | OnTouchEnd(`RagdollHand` ragdollHand) |  | 
| `void` | OnTouchStart(`RagdollHand` ragdollHand) |  | 
| `void` | ShowHint(`RagdollHand` ragdollHand) |  | 
| `Boolean` | TryTouchAction(`RagdollHand` ragdollHand, `Action` action) |  | 


## `WheelMenu`

```csharp
public class ThunderRoad.WheelMenu
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `EffectInstance` | centerEffectInstance |  | 
| `Boolean` | isShown |  | 
| `Int32` | layer |  | 
| `Single` | orbRadius |  | 
| `List<Orb>` | orbs |  | 
| `Orb` | selectedOrb |  | 
| `String` | selectionEffectStepCustomId |  | 
| `Int32` | selectionHashId |  | 
| `Transform` | selector |  | 
| `Boolean` | selectorActive |  | 
| `Single` | selectorDistanceFromCenter |  | 
| `Single` | selectorMinRadius |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `Vector3` | GetOrbLocalPosition(`Int32` orbIndex, `Single` startAngle, `Single` maxAngle, `Boolean` uniform = True, `Boolean` revert = False) |  | 
| `void` | Hide() |  | 
| `void` | OnOrbSelected(`Orb` orb, `Boolean` active) |  | 
| `void` | Show(`EffectData` centerEffectData, `List<Orb>` orbs, `Single` startAngle = 0, `Single` maxAngle = 360, `Boolean` uniform = True, `Boolean` revert = False) |  | 
| `void` | Show(`Vector3` position, `EffectData` centerEffectData, `List<Orb>` orbs, `Single` startAngle = 0, `Single` maxAngle = 360, `Boolean` uniform = True, `Boolean` revert = False) |  | 
| `void` | TestShow(`Int32` count, `Single` startAngle = 0, `Single` maxAngle = 360, `Boolean` uniform = True, `Boolean` revert = False) |  | 
| `void` | Update() |  | 


## `WheelMenuInventory`

```csharp
public class ThunderRoad.WheelMenuInventory
    : WheelMenu

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | Hide() |  | 
| `void` | Show() |  | 


## `WheelMenuSpell`

```csharp
public class ThunderRoad.WheelMenuSpell
    : WheelMenu

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Player` | player |  | 
| `Side` | side |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | Hide() |  | 
| `void` | OnDisable() |  | 
| `void` | Show() |  | 
| `void` | Update() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `WheelMenuSpell` | left |  | 
| `WheelMenuSpell` | right |  | 


## `WhooshEffect`

```csharp
public class ThunderRoad.WhooshEffect
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | dampenedIntensity |  | 
| `Single` | dampening |  | 
| `Boolean` | effectActive |  | 
| `FxController` | effectMixer |  | 
| `Item` | item |  | 
| `Single` | maxVelocity |  | 
| `Single` | minVelocity |  | 
| `Rigidbody` | rb |  | 
| `Boolean` | started |  | 
| `Boolean` | stopOnSnap |  | 
| `List<GameObject>` | toggleGameobjects |  | 
| `Trigger` | trigger |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Init() |  | 
| `void` | OnDisable() |  | 
| `void` | OnEnable() |  | 
| `void` | OnObjectGrabbed(`Handle` handle, `RagdollHand` ragdollHand) |  | 
| `void` | OnObjectReleased(`Handle` handle, `RagdollHand` ragdollHand, `Boolean` forSnap) |  | 
| `void` | OnSnap(`Holder` holder) |  | 
| `void` | OnThrowingEnded() |  | 
| `void` | OnThrowingStarted() |  | 
| `void` | Update() |  | 


## `WhooshPoint`

```csharp
public class ThunderRoad.WhooshPoint
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | dampenedIntensity |  | 
| `Single` | dampening |  | 
| `Boolean` | effectActive |  | 
| `EffectData` | effectData |  | 
| `EffectInstance` | effectInstance |  | 
| `Item` | item |  | 
| `Single` | maxVelocity |  | 
| `Single` | minVelocity |  | 
| `Rigidbody` | rb |  | 
| `Boolean` | stopOnSnap |  | 
| `Trigger` | trigger |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Load(`EffectData` effectData, `Whoosh` whooshData) |  | 
| `void` | OnDisable() |  | 
| `void` | OnEnable() |  | 
| `void` | OnObjectGrabbed(`Handle` handle, `RagdollHand` ragdollHand) |  | 
| `void` | OnObjectReleased(`Handle` handle, `RagdollHand` ragdollHand, `Boolean` forSnap) |  | 
| `void` | OnSnap(`Holder` holder) |  | 
| `void` | OnThrowingEnded() |  | 
| `void` | OnThrowingStarted() |  | 
| `void` | Update() |  | 


## `WristRelaxer`

```csharp
public class ThunderRoad.WristRelaxer
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Transform` | armTwistBone |  | 
| `Transform` | handBone |  | 
| `Transform` | lowerArmBone |  | 
| `Single` | parentChildCrossfade |  | 
| `RagdollHand` | ragdollHand |  | 
| `Single` | twistAngleOffset |  | 
| `Transform` | upperArmBone |  | 
| `Single` | weight |  | 
| `Single` | weightArm |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | Init() |  | 


## `WristStats`

```csharp
public class ThunderRoad.WristStats
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Creature` | creature |  | 
| `EffectData` | focusEffectData |  | 
| `String` | focusEffectId |  | 
| `EffectInstance` | focusEffectInstance |  | 
| `EffectData` | healthEffectData |  | 
| `String` | healthEffectId |  | 
| `Boolean` | isShown |  | 
| `EffectInstance` | lifeEffectInstance |  | 
| `EffectData` | manaEffectData |  | 
| `String` | manaEffectId |  | 
| `EffectInstance` | manaEffectInstance |  | 
| `Single` | showAngle |  | 
| `Single` | showDistance |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `List<ValueDropdownItem<String>>` | GetAllEffectID() |  | 
| `void` | InitEffects() |  | 
| `void` | OnPossessionEvent(`Creature` creature, `EventTime` eventTime) |  | 
| `void` | Show(`Boolean` active) |  | 


## `Zone`

```csharp
public class ThunderRoad.Zone
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `ZoneEvent` | creatureEnterEvent |  | 
| `ZoneEvent` | creatureExitEvent |  | 
| `Transform` | customTeleportTarget |  | 
| `Single` | despawnDelay |  | 
| `Boolean` | despawnItem |  | 
| `Boolean` | despawnNPC |  | 
| `String` | effectID |  | 
| `AnimationCurve` | effectMassVelocityCurve |  | 
| `Vector3` | effectOrientation |  | 
| `ZoneEvent` | itemEnterEvent |  | 
| `ZoneEvent` | itemExitEvent |  | 
| `Boolean` | killNPC |  | 
| `Boolean` | killPlayer |  | 
| `Boolean` | navSpeedModifier |  | 
| `ZoneEvent` | playerEnterEvent |  | 
| `ZoneEvent` | playerExitEvent |  | 
| `Single` | runSpeed |  | 
| `Boolean` | spawnEffect |  | 
| `Boolean` | teleportItem |  | 
| `Boolean` | teleportPlayer |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | TestEvent(`Object` obj) |  | 


## `ZoneViewEnabler`

```csharp
public class ThunderRoad.ZoneViewEnabler
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | target |  | 
| `List<BoxCollider>` | workingZones |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ExecuteBeforeCameraRender(`ScriptableRenderContext` context, `Camera` camera) |  | 


