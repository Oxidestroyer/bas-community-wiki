# ThunderRoad.AI

## `ActionNode`

```csharp
public class ThunderRoad.AI.ActionNode
    : Node

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Blackboard` | blackboard |  | 
| `BrainData` | brainData |  | 
| `Creature` | creature |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 


## `BehaviorTreeData`

```csharp
public class ThunderRoad.AI.BehaviorTreeData
    : CatalogData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Blackboard` | blackboard |  | 
| `Creature` | creature |  | 
| `String` | lastDebugString |  | 
| `Node` | rootNode |  | 
| `Type` | type |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard = null) |  | 
| `Boolean` | IsRunningNode() |  | 
| `void` | OnDrawGizmos() |  | 
| `void` | OnDrawGizmosSelected() |  | 
| `State` | PassThrough() |  | 
| `void` | Reset() |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `BehaviorTreeData` | Instantiate(`String` treeID) |  | 


## `Blackboard`

```csharp
public class ThunderRoad.AI.Blackboard

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<IDictionary>` | dictionaries |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | Exist(`String` s) |  | 
| `T` | Find(`String` s) |  | 
| `void` | UpdateBB() |  | 
| `void` | UpdateVariable(`String` s, `T` variable) |  | 


## `ChildTreeNode`

```csharp
public class ThunderRoad.AI.ChildTreeNode
    : Node

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | childTreeID |  | 
| `String` | childTreeName |  | 
| `ChildNodeRef` | reference |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Node` | Clone() |  | 
| `State` | Evaluate() |  | 
| `List<ValueDropdownItem<String>>` | GetAllBehaviorTreeID() |  | 
| `String` | GetDebugString() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 
| `Boolean` | IsRunningNode() |  | 
| `void` | OnDrawGizmos() |  | 
| `void` | OnDrawGizmosSelected() |  | 
| `void` | Reset() |  | 


## `ConditionNode`

```csharp
public abstract class ThunderRoad.AI.ConditionNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Blackboard` | blackboard |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ConditionNode` | Clone() |  | 
| `Boolean` | Evaluate() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 


## `ControlNode`

```csharp
public class ThunderRoad.AI.ControlNode
    : Node

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Node>` | childs |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Node` | Clone() |  | 
| `String` | GetChildsDebugString() |  | 
| `String` | GetDebugString() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 
| `Boolean` | IsRunningNode() |  | 
| `void` | OnDrawGizmos() |  | 
| `void` | OnDrawGizmosSelected() |  | 


## `DecoratorNode`

```csharp
public class ThunderRoad.AI.DecoratorNode
    : Node

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Node` | child |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Node` | Clone() |  | 
| `State` | Evaluate() |  | 
| `String` | GetDebugString() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 
| `Boolean` | IsRunningNode() |  | 
| `void` | OnDrawGizmos() |  | 
| `void` | OnDrawGizmosSelected() |  | 
| `void` | Reset() |  | 


## `Node`

```csharp
public class ThunderRoad.AI.Node

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | nodeState |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Node` | Clone() |  | 
| `State` | Evaluate() |  | 
| `String` | GetDebugString() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 
| `Boolean` | IsRunningNode() |  | 
| `void` | OnDrawGizmos() |  | 
| `void` | OnDrawGizmosSelected() |  | 
| `void` | OnFail() |  | 
| `void` | OnRun() |  | 
| `void` | OnSuccess() |  | 
| `void` | Reset() |  | 


## `State`

```csharp
public enum ThunderRoad.AI.State
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | SUCCESS |  | 
| `1` | FAILURE |  | 
| `2` | RUNNING |  | 


