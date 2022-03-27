# ThunderRoad.AI.Get

## `AvailableWeapons`

```csharp
public class ThunderRoad.AI.Get.AvailableWeapons

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Item` | bow |  | 
| `Item` | leftMelee1h |  | 
| `Item` | melee2h |  | 
| `Single` | meleeDistance1h |  | 
| `Single` | meleeDistance2h |  | 
| `Item` | rightMelee1h |  | 
| `Item` | shield |  | 
| `SpellData` | spell |  | 


## `GetAvailableWeapons`

```csharp
public class ThunderRoad.AI.Get.GetAvailableWeapons
    : ActionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AvailableWeapons` | availableWeapons |  | 
| `String` | outputAvailableAttacksVariableName |  | 
| `List<String>` | priorityTreeID |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CheckWeapon(`Item` weapon, `Single&` greaterReach, `Single&` secondReach) |  | 
| `State` | Evaluate() |  | 
| `List<ValueDropdownItem<String>>` | GetAllSubTreesID() |  | 


## `GetCreature`

```csharp
public class ThunderRoad.AI.Get.GetCreature
    : ActionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | checkFov |  | 
| `Boolean` | checkShortestPath |  | 
| `Boolean` | checkSight |  | 
| `Creature` | creatureFound |  | 
| `Boolean` | debugLines |  | 
| `List<Creature>` | filteredCreatures |  | 
| `List<RagdollPart>` | filteredRagdollParts |  | 
| `Single` | maxDistance |  | 
| `BrainModuleDetection` | moduleDetection |  | 
| `Boolean` | outputCreatureAsCurrentTarget |  | 
| `String` | outputCreatureVariableName |  | 
| `OutputTransform` | outputTransform |  | 
| `String` | outputTransformVariableName |  | 
| `RagdollPart` | ragdollPartSighted |  | 
| `Single` | rememberDuration |  | 
| `Single` | rememberTime |  | 
| `Target` | target |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 
| `void` | OutputClearVariables() |  | 
| `void` | Reset() |  | 


## `GetCreaturePart`

```csharp
public class ThunderRoad.AI.Get.GetCreaturePart
    : ActionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Creature` | inputCreature |  | 
| `String` | inputCreatureVariableName |  | 
| `Transform` | outputTransform |  | 
| `String` | outputTransformVariableName |  | 
| `Target` | target |  | 
| `TargetPart` | targetPart |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 
| `void` | Reset() |  | 


## `GetItem`

```csharp
public class ThunderRoad.AI.Get.GetItem
    : ActionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | avoidTargetRadius |  | 
| `List<Handle>` | closestItemHandles |  | 
| `Side` | handleSide |  | 
| `String` | outputItemHandleTransformVariableName |  | 
| `String` | outputItemHandleVariableName |  | 
| `Type` | type |  | 
| `Boolean` | useShortestPath |  | 
| `WeaponClass` | weaponClass |  | 
| `WeaponHandling` | weaponHandling |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `Boolean` | HandleNearThreat(`Handle` handle) |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 
| `void` | Reset() |  | 


## `GetNoisePosition`

```csharp
public class ThunderRoad.AI.Get.GetNoisePosition
    : ActionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BrainModuleDetection` | moduleDetection |  | 
| `NavMeshPath` | navMeshPath |  | 
| `Noise` | noise |  | 
| `Single` | offsetHeightRatioWhenOnFloor |  | 
| `String` | outputOffsetPositionVariableName |  | 
| `String` | outputPositionVariableName |  | 
| `Single` | raycastOffset |  | 
| `Single` | rememberTime |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 


## `GetRandomPositionAround`

```csharp
public class ThunderRoad.AI.Get.GetRandomPositionAround
    : ActionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | inputTargetVariableName |  | 
| `Single` | maxRadius |  | 
| `Single` | minRadius |  | 
| `Creature` | moveTargetCreature |  | 
| `Vector3` | moveTargetPosition |  | 
| `Transform` | moveTargetTransform |  | 
| `NavMeshPath` | navMeshPath |  | 
| `String` | outputPositionVariableName |  | 
| `Target` | target |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `Vector3` | GetRandomPointAround(`Vector3` position, `Single` minRadius, `Single` maxRadius) |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 


## `GetSharedTarget`

```csharp
public class ThunderRoad.AI.Get.GetSharedTarget
    : ActionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | checkCloseFriends |  | 
| `Boolean` | checkRoomAlert |  | 
| `Boolean` | checkShortestPath |  | 
| `Single` | closeFriendMaxDistance |  | 
| `Creature` | creatureFound |  | 
| `List<Creature>` | filteredCreatures |  | 
| `Boolean` | outputCreatureAsCurrentTarget |  | 
| `String` | outputCreatureVariableName |  | 
| `String` | outputTransformVariableName |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 
| `void` | OutputClearVariables() |  | 
| `void` | Reset() |  | 


## `GetShootPoint`

```csharp
public class ThunderRoad.AI.Get.GetShootPoint
    : ActionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | checkShortestPath |  | 
| `ShootPoint` | currentShootPoint |  | 
| `String` | inputVariableName |  | 
| `NavMeshPath` | navMeshPath |  | 
| `String` | outputPositionVariableName |  | 
| `Target` | target |  | 
| `Creature` | targetCreature |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `ShootPoint` | GetClosest(`ShootPoint[]` shootPoints, `Int32` shootPointCount, `Vector3` position, `Boolean` prioritizeShortestPath) |  | 
| `void` | Reset() |  | 


## `GetShootPosition`

```csharp
public class ThunderRoad.AI.Get.GetShootPosition
    : ActionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | checkShortestPath |  | 
| `ShootPosition` | currentShootPosition |  | 
| `String` | inputVariableName |  | 
| `NavMeshPath` | navMeshPath |  | 
| `String` | outputPositionVariableName |  | 
| `Target` | target |  | 
| `Creature` | targetCreature |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `ShootPosition` | GetClosestShootPositionIndex(`ShootPosition[]` shootPositions, `Vector3` position, `Boolean` checkShortestPath) |  | 
| `void` | Reset() |  | 


## `GetTransform`

```csharp
public class ThunderRoad.AI.Get.GetTransform
    : ActionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Transform>` | closestTransforms |  | 
| `BrainModulePatrol` | modulePatrol |  | 
| `String` | outputTransformVariableName |  | 
| `Boolean` | prioritizeShortestPath |  | 
| `Target` | target |  | 
| `Transform` | transform |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 
| `void` | Reset() |  | 


## `SelectSpell`

```csharp
public class ThunderRoad.AI.Get.SelectSpell
    : ActionNode

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CalculateWeight(`List<Choice>` listChoice) |  | 
| `State` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 
| `Choice` | PickChoice(`List<Choice>` listChoice, `Int32` pickCount = 0) |  | 


