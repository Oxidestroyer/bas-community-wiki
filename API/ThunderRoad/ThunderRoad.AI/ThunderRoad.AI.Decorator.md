# ThunderRoad.AI.Decorator

## `AlwaysFailure`

```csharp
public class ThunderRoad.AI.Decorator.AlwaysFailure
    : DecoratorNode

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 


## `AlwaysRunning`

```csharp
public class ThunderRoad.AI.Decorator.AlwaysRunning
    : DecoratorNode

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 


## `AlwaysSuccess`

```csharp
public class ThunderRoad.AI.Decorator.AlwaysSuccess
    : DecoratorNode

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 


## `IfCondition`

```csharp
public class ThunderRoad.AI.Decorator.IfCondition
    : DecoratorNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | conditionResult |  | 
| `List<ConditionNode>` | ifConditions |  | 
| `List<ConditionNode>` | ifNotConditions |  | 
| `Operation` | operation |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `String` | GetDebugString() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 


## `Inverter`

```csharp
public class ThunderRoad.AI.Decorator.Inverter
    : DecoratorNode

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 


## `Loop`

```csharp
public class ThunderRoad.AI.Decorator.Loop
    : DecoratorNode

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Node` | loopingNode |  | 
| `Mode` | mode |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Node` | Clone() |  | 
| `State` | Evaluate() |  | 
| `String` | GetDebugString() |  | 
| `void` | Init(`Creature` p_creature, `Blackboard` p_blackboard) |  | 
| `Boolean` | IsRunningNode() |  | 
| `void` | Reset() |  | 


## `NoReset`

```csharp
public class ThunderRoad.AI.Decorator.NoReset
    : DecoratorNode

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `State` | Evaluate() |  | 
| `void` | Reset() |  | 


