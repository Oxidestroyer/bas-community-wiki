# ThunderRoad.AI.Action

## `AttackBow`

```csharp
public class ThunderRoad.AI.Action.AttackBow
    : ActionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Transform` | aimAnchor |  | 
| `Single` | aimArmSpringMultiplier |  | 
| `Coroutine` | aimCoroutine |  | 
| `Single` | aimDelay |  | 
| `Transform` | aimHandle |  | 
| `Boolean` | aimOnTarget |  | 
| `Single` | aimTime |  | 
| `Transform` | aimTransform |  | 
| `BowString` | bowString |  | 
| `String` | inputTransformVariableName |  | 
| `Single` | lastBowAimTime |  | 
| `BrainModuleBow` | moduleBow |  | 
| `BrainModuleDetection` | moduleDetection |  | 
| `BrainModuleEquipment` | moduleEquipment |  | 
| `BrainModuleMove` | moduleMove |  | 
| `Single` | nextBowAimDelay |  | 
| `Transform` | shootTarget |  | 
| `BowState` | state |  | 
| `Creature` | targetCreature |  | 
| `Transform` | targetTransform |  | 
| `Boolean` | useCurrentTargetIfNullTransform |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AimSpread(`Boolean` instant = False) |  | 
| `State` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 
| `void` | OnBowShoot(`Item` arrow) |  | 
| `void` | OnFail() |  | 
| `void` | OnRagdollStateChange(`State` previousState, `State` newState, `PhysicStateChange` physicStateChange, `EventTime` eventTime) |  | 
| `void` | OnRun() |  | 
| `void` | Reset() |  | 
| `void` | StopShooting() |  | 


## `AttackMelee`

```csharp
public class ThunderRoad.AI.Action.AttackMelee
    : ActionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Clip` | animationDataClip |  | 
| `Boolean` | attackDone |  | 
| `Boolean` | checkCloseAllies |  | 
| `Boolean` | checkCurrentTargetSight |  | 
| `Single` | forceMaxRangeDelta |  | 
| `Single` | forceMeleeRange |  | 
| `Single` | forceMeleeRangeMoved |  | 
| `Single` | forceWeaponReach |  | 
| `String` | inputTransformVariableName |  | 
| `BrainModuleDetection` | moduleDetection |  | 
| `BrainModuleEquipment` | moduleEquipment |  | 
| `BrainModuleMelee` | moduleMelee |  | 
| `BrainModuleMove` | moduleMove |  | 
| `BrainModuleStance` | moduleStance |  | 
| `Vector3` | orgAttackDirection |  | 
| `Int32` | pickClipSequentialMaxIndex |  | 
| `Int32` | sequentialIndex |  | 
| `Boolean` | stopOnReset |  | 
| `Target` | target |  | 
| `Transform` | targetTransform |  | 
| `Boolean` | updateClipRange |  | 
| `Vector3` | updateClipRangeStartPosition |  | 
| `Quaternion` | updateClipRangeStartRotation |  | 
| `Boolean` | useMeleeDelay |  | 
| `Item` | weapon |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 
| `void` | OnAttackUpdate() |  | 
| `void` | OnDrawGizmos() |  | 
| `void` | OnKill(`CollisionInstance` collisionInstance, `EventTime` eventTime) |  | 
| `void` | OnRagdollStateChange(`State` previousState, `State` newState, `PhysicStateChange` physicStateChange, `EventTime` eventTime) |  | 
| `void` | OnRun() |  | 
| `void` | OnWeaponCollision(`CollisionInstance` collisionInstance) |  | 
| `void` | Reset() |  | 
| `void` | StopAttack() |  | 


## `AttackSpell`

```csharp
public class ThunderRoad.AI.Action.AttackSpell
    : ActionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Transform` | aimLeft |  | 
| `Transform` | aimLeftHandAnchor |  | 
| `Transform` | aimRight |  | 
| `Transform` | aimRightHandAnchor |  | 
| `Boolean` | castLeft |  | 
| `Coroutine` | castLeftCoroutine |  | 
| `Boolean` | castRight |  | 
| `Coroutine` | castRightCoroutine |  | 
| `String` | inputTransformVariableName |  | 
| `SpellCastData[]` | inRangeSpell |  | 
| `Int32` | inRangeSpellCount |  | 
| `BrainModuleCast` | moduleCast |  | 
| `BrainModuleDetection` | moduleDetection |  | 
| `BrainModuleEquipment` | moduleEquipment |  | 
| `BrainModuleMove` | moduleMove |  | 
| `Single` | nextCastDelay |  | 
| `Target` | target |  | 
| `Transform` | targetTransform |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 
| `void` | OnFail() |  | 
| `void` | Reset() |  | 
| `void` | StopCast() |  | 


## `CanDrawItem`

```csharp
public class ThunderRoad.AI.Action.CanDrawItem
    : ActionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | checkAmmo |  | 
| `Coroutine` | drawCoroutine |  | 
| `Boolean` | drawLeftWeapon |  | 
| `Boolean` | drawRightWeapon |  | 
| `Coroutine` | holsterCoroutine |  | 
| `Boolean` | leftSideOk |  | 
| `WeaponClass` | leftWeaponClass |  | 
| `Item` | leftWeaponToDraw |  | 
| `BrainModuleEquipment` | moduleEquipment |  | 
| `Boolean` | rightSideOk |  | 
| `WeaponClass` | rightWeaponClass |  | 
| `WeaponHandling` | rightWeaponHandling |  | 
| `Item` | rightWeaponToDraw |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CheckLeftWeapon(`Item` weapon) |  | 
| `Boolean` | CheckRightWeapon(`Item` weapon) |  | 
| `State` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 


## `ChickenFallingNode`

```csharp
public class ThunderRoad.AI.Action.ChickenFallingNode
    : ActionNode

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 


## `Despawn`

```csharp
public class ThunderRoad.AI.Action.Despawn
    : ActionNode

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 


## `DrawItem`

```csharp
public class ThunderRoad.AI.Action.DrawItem
    : CanDrawItem

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `void` | OnFail() |  | 
| `void` | Reset() |  | 
| `void` | StopDraw() |  | 


## `HasSpell`

```csharp
public class ThunderRoad.AI.Action.HasSpell
    : ConditionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Creature` | creature |  | 
| `String` | spellID |  | 
| `Single` | spellMaxDistance |  | 
| `Single` | spellMinDistance |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 


## `HolsterItem`

```csharp
public class ThunderRoad.AI.Action.HolsterItem
    : ActionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Coroutine` | holsterCoroutine |  | 
| `Boolean` | holsterLeft |  | 
| `Boolean` | holsterRight |  | 
| `BrainModuleEquipment` | moduleEquipment |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 
| `void` | OnFail() |  | 
| `void` | Reset() |  | 
| `void` | StopHolster() |  | 


## `IsGrabbing`

```csharp
public class ThunderRoad.AI.Action.IsGrabbing
    : ConditionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Creature` | creature |  | 
| `Side` | hand |  | 
| `WeaponClass` | weaponClass |  | 
| `Filter` | weaponClassFilter |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 


## `MoveTo`

```csharp
public class ThunderRoad.AI.Action.MoveTo
    : ActionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AngleMode` | angleMode |  | 
| `Single` | approachMoveSpeedRatio |  | 
| `Single` | approachRunSpeedRatio |  | 
| `Single` | approachTurnSpeedRatio |  | 
| `AutoRadius` | autoRadius |  | 
| `Boolean` | changeAngleUntilUnobstructed |  | 
| `Boolean` | checkMaxAllies |  | 
| `Single` | firstToSecondRadiusDistance |  | 
| `Boolean` | forceTurnToUseMoveDirectionAtDistance |  | 
| `String` | inputMoveTargetVariableName |  | 
| `String` | inputTurnTargetVariableName |  | 
| `Vector3` | lastPosition |  | 
| `BrainModuleDetection` | moduleDetection |  | 
| `BrainModuleMelee` | moduleMelee |  | 
| `BrainModuleMove` | moduleMove |  | 
| `Boolean` | moveCloserIfNoSight |  | 
| `MoveTarget` | moveTarget |  | 
| `Creature` | moveTargetCreature |  | 
| `Vector3` | moveTargetPosition |  | 
| `Transform` | moveTargetTransform |  | 
| `Single` | repathMaxDelay |  | 
| `Single` | repathMinDelay |  | 
| `Single` | secondRadiusRange |  | 
| `Boolean` | strafeAroundTarget |  | 
| `Single` | strafeMoveSpeedRatio |  | 
| `Single` | strafeRunSpeedRatio |  | 
| `Single` | strafeTurnSpeedRatio |  | 
| `Single` | stuckDuration |  | 
| `Single` | stuckMaxDuration |  | 
| `Single` | stuckRadius |  | 
| `Single` | targetMaxRadius |  | 
| `Single` | targetMinRadius |  | 
| `Single` | targetRadiusMaxAngle |  | 
| `Single` | targetRadiusMinAngle |  | 
| `Single` | turnMoveDirectionDistance |  | 
| `Single` | turnMoveDirectionSpeed |  | 
| `TurnTarget` | turnTarget |  | 
| `Transform` | turnTargetTransform |  | 
| `Boolean` | useModuleStrafeDelay |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 
| `void` | OnDrawGizmos() |  | 
| `void` | OnFail() |  | 
| `void` | OnSuccess() |  | 
| `void` | Reset() |  | 
| `void` | Stop() |  | 
| `void` | Turn() |  | 


## `PickupItem`

```csharp
public class ThunderRoad.AI.Action.PickupItem
    : ActionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | angle |  | 
| `Coroutine` | coroutine |  | 
| `Single` | distance |  | 
| `Boolean` | done |  | 
| `Boolean` | fail |  | 
| `Single` | grabbedHeight |  | 
| `Vector3` | grabPosition |  | 
| `Single` | grabTime |  | 
| `Transform` | ikTarget |  | 
| `String` | inputItemHandleVariableName |  | 
| `Boolean` | isGrabbing |  | 
| `Handle` | itemHandle |  | 
| `AnimationData` | pickupAnimationData |  | 
| `String` | pickupAnimationId |  | 
| `Single` | pickupDuration |  | 
| `Single` | pickupIKDuration |  | 
| `Side` | side |  | 
| `Single` | standUpTime |  | 
| `Boolean` | useIK |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `List<ValueDropdownItem<String>>` | GetAllAnimationID() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 
| `void` | OnFail() |  | 
| `void` | OnRun() |  | 
| `void` | Reset() |  | 
| `void` | StopGrabbing() |  | 


## `PlayerDetectionNode`

```csharp
public class ThunderRoad.AI.Action.PlayerDetectionNode
    : ActionNode

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 
| `void` | OnDrawGizmos() |  | 


## `SetAnimator`

```csharp
public class ThunderRoad.AI.Action.SetAnimator
    : ActionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | boolValue |  | 
| `Single` | floatValue |  | 
| `String` | parameterID |  | 
| `Parameter` | parameterType |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 


## `SetBrainState`

```csharp
public class ThunderRoad.AI.Action.SetBrainState
    : ActionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | brainState |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 


## `SetDodge`

```csharp
public class ThunderRoad.AI.Action.SetDodge
    : ActionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `DodgeBehaviour` | dodgeBehaviour |  | 
| `String` | inputCreatureVariableName |  | 
| `BrainModuleDodge` | moduleDodge |  | 
| `Target` | target |  | 
| `Creature` | targetCreature |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 


## `SetLookAt`

```csharp
public class ThunderRoad.AI.Action.SetLookAt
    : ActionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | enabled |  | 
| `String` | inputVariableName |  | 
| `Vector3` | lookPosition |  | 
| `Transform` | lookTarget |  | 
| `BrainModuleLookAt` | moduleLookAt |  | 
| `Target` | target |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 
| `void` | OnFail() |  | 
| `void` | Reset() |  | 
| `void` | Stop() |  | 


## `SetParry`

```csharp
public class ThunderRoad.AI.Action.SetParry
    : ActionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | enabled |  | 
| `String` | inputCreatureVariableName |  | 
| `BrainModuleParry` | moduleParry |  | 
| `Target` | target |  | 
| `Creature` | targetCreature |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 
| `void` | OnFail() |  | 
| `void` | Reset() |  | 


## `SetStance`

```csharp
public class ThunderRoad.AI.Action.SetStance
    : ActionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BrainModuleStance` | moduleStance |  | 
| `Stance` | stance |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 


## `Speak`

```csharp
public class ThunderRoad.AI.Action.Speak
    : ActionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | abnormalNoise |  | 
| `Int32` | dialogHashId |  | 
| `String` | dialogId |  | 
| `Boolean` | ignoreIfFromWave |  | 
| `BrainModuleSpeak` | moduleSpeak |  | 
| `Boolean` | onlyOnce |  | 
| `Boolean` | played |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 
| `void` | Reset() |  | 


## `TurnTo`

```csharp
public class ThunderRoad.AI.Action.TurnTo
    : ActionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BrainModuleMove` | brainModuleMove |  | 
| `String` | inputVariableName |  | 
| `Single` | successAngle |  | 
| `Boolean` | successIfAngleReached |  | 
| `Target` | target |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 
| `void` | OnFail() |  | 
| `void` | OnSuccess() |  | 
| `void` | Reset() |  | 
| `void` | Stop() |  | 


## `Wait`

```csharp
public class ThunderRoad.AI.Action.Wait
    : ActionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | isWaiting |  | 
| `Single` | maxDuration |  | 
| `Single` | minDuration |  | 
| `Single` | waitDuration |  | 
| `Single` | waitTime |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `void` | Reset() |  | 


## `WayPointTask`

```csharp
public class ThunderRoad.AI.Action.WayPointTask
    : ActionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | animationRandomDelay |  | 
| `Single` | animationStartTime |  | 
| `String` | inputTransformVariableName |  | 
| `BrainModuleMove` | moduleMove |  | 
| `BrainModulePatrol` | modulePatrol |  | 
| `Single` | startTime |  | 
| `Single` | stopDelay |  | 
| `Boolean` | waitTurn |  | 
| `WayPoint` | wayPoint |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 
| `void` | Reset() |  | 
| `void` | UpdateTurn() |  | 


