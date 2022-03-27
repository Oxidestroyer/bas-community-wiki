# ThunderRoad.AI.Condition

## `BlackboardValue`

```csharp
public class ThunderRoad.AI.Condition.BlackboardValue
    : ConditionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | comparedValue |  | 
| `Creature` | creature |  | 
| `Comparator` | variableComparator |  | 
| `String` | variableName |  | 
| `VariableType` | variableType |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 


## `IfTooMuchAllies`

```csharp
public class ThunderRoad.AI.Condition.IfTooMuchAllies
    : ConditionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | attackingOnly |  | 
| `Creature` | creature |  | 
| `BrainModuleDetection` | moduleDetection |  | 
| `BrainModuleMelee` | moduleMelee |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 


## `IsAlerted`

```csharp
public class ThunderRoad.AI.Condition.IsAlerted
    : ConditionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Creature` | creature |  | 
| `Boolean` | isAlerted |  | 
| `BrainModulePatrol` | modulePatrol |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 


## `IsFromWave`

```csharp
public class ThunderRoad.AI.Condition.IsFromWave
    : ConditionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Creature` | creature |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 


## `IsMeleeChosen`

```csharp
public class ThunderRoad.AI.Condition.IsMeleeChosen
    : ConditionNode

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | Evaluate() |  | 


## `IsPushed`

```csharp
public class ThunderRoad.AI.Condition.IsPushed
    : ConditionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Creature` | creature |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 


## `IsThreatned`

```csharp
public class ThunderRoad.AI.Condition.IsThreatned
    : ConditionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Creature` | creature |  | 
| `String` | inputCreatureVariableName |  | 
| `Single` | lastThreatTime |  | 
| `BrainModuleDetection` | moduleDetection |  | 
| `Target` | target |  | 
| `Creature` | targetCreature |  | 
| `Single` | threatDuration |  | 
| `Single` | threatMinSpeed |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 


## `IsUnarmed`

```csharp
public class ThunderRoad.AI.Condition.IsUnarmed
    : ConditionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Creature` | creature |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 


