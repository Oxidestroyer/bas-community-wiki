# ThunderRoad.AI.Control

## `Parallel`

```csharp
public class ThunderRoad.AI.Control.Parallel
    : ControlNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | failureCount |  | 
| `State[]` | nodeStates |  | 
| `Boolean` | stopOnFirstFailure |  | 
| `Boolean` | stopOnFirstSuccess |  | 
| `Int32` | successCount |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `String` | GetChildsDebugString() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 
| `void` | Reset() |  | 


## `Selector`

```csharp
public class ThunderRoad.AI.Control.Selector
    : ControlNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | evaluateAllNodesOnCycle |  | 
| `Int32` | nodeIndex |  | 
| `Int32` | previousNodeIndex |  | 
| `Int32` | runningNodeIndex |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `String` | GetChildsDebugString() |  | 
| `void` | Reset() |  | 


## `Sequence`

```csharp
public class ThunderRoad.AI.Control.Sequence
    : ControlNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | evaluateAllNodesOnCycle |  | 
| `Int32` | nodeIndex |  | 
| `Int32` | previousNodeIndex |  | 
| `Int32` | runningNodeIndex |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `String` | GetChildsDebugString() |  | 
| `void` | Reset() |  | 


