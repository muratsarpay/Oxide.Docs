---
title: Structure Hooks
---

# Structure Hooks

## OnCodeEntered

``` csharp
object OnCodeEntered(CodeLock codeLock, BasePlayer player, string code)
{
    Puts("OnCodeEntered works!");
    return null;
}
```

 * Called when the player has entered a code in a codelock
 * Returning a non-null value overrides default behavior

## OnCupboardAuthorize

``` csharp
object OnCupboardAuthorize(BuildingPrivlidge privilege, BasePlayer player)
{
    Puts("OnCupboardAuthorize works!");
    return null;
}
```

 * Called when a cupboard attempts to authorize a player
 * Returning a non-null value overrides default behavior

## OnCupboardClearList

``` csharp
object OnCupboardClearList(BuildingPrivlidge privilege, BasePlayer player)
{
    Puts("OnCupboardClearList works!");
    return null;
}
```

 * Called when an attempt is made to clear a cupboard authorized list
 * Returning a non-null value overrides default behavior

## OnCupboardDeauthorize

``` csharp
object OnCupboardDeauthorize(BuildingPrivlidge privilege, BasePlayer player)
{
    Puts("OnCupboardDeauthorize works!");
    return null;
}
```

 * Called when a cupboard attempts to deauthorize a player
 * Returning a non-null value overrides default behavior

## OnDoorClosed

``` csharp
void OnDoorClosed(Door door, BasePlayer player)
{
    Puts("OnDoorClosed works!");
}
```

 * Called when the player closed a door
 * No return behavior

## OnDoorOpened

``` csharp
void OnDoorOpened(Door door, BasePlayer player)
{
    Puts("OnDoorOpened works!");
}
```

 * Called when the player opened a door
 * No return behavior

## OnDoorKnocked

``` csharp
void OnDoorKnocked(Door door, BasePlayer player)
{
    Puts("OnDoorKnocked works!");
}
```

 * Called when the player knocks on a door
 * No return behavior

## OnEntityBuilt

``` csharp
void OnEntityBuilt(Planner plan, GameObject go)
{
    Puts("OnEntityBuilt works!");
}
```

 * Called when any structure is built (walls, ceilings, stairs, etc.)
 * No return behavior

## OnHammerHit

``` csharp
void OnHammerHit(BasePlayer player, HitInfo info)
{
    Puts("OnHammerHit works!");
}
```

 * Called when the player has hit something with a hammer
 * No return behavior

## OnStructureDemolish

``` csharp
object OnStructureDemolish(BaseCombatEntity entity, BasePlayer player)
{
    Puts("OnStructureDemolish works!");
    return null;
}
```

 * Called when the player selects DemolishImmediate from the BuildingBlock or BaseCombatEntity menu
 * Returning a non-null value overrides default behavior

## OnStructureRepair

``` csharp
void OnStructureRepair(BaseCombatEntity entity, BasePlayer player)
{
    Puts("OnStructureRepair works!");
}
```

 * Called when the player repairs a BuildingBlock or BaseCombatEntity
 * No return behavior

## OnStructureRotate

``` csharp
void OnStructureRotate(BaseCombatEntity entity, BasePlayer player)
{
    Puts("OnStructureRotate works!");
}
```

 * Called when the player rotates a BuildingBlock or BaseCombatEntity
 * No return behavior

## OnStructureUpgrade

``` csharp
object OnStructureUpgrade(BaseCombatEntity entity, BasePlayer player, BuildingGrade.Enum grade)
{
    Puts("OnStructureUpgrade works!");
    return null;
}
```

 * Called when the player upgrades the grade of a BuildingBlock or BaseCombatEntity
 * Returning a non-null value overrides default behavior
