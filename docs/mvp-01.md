# MVP 1: Wood and Construction Loop

## Goal

The goal of MVP 1 is to create the smallest playable prototype that proves the basic construction and wood production loop works.

MVP 1 should answer this question:

> Is it understandable and satisfying to use Wood to construct buildings that produce more resources over time?

MVP 1 is not meant to be a full game.

It is a test of the basic economy foundation:

- Wood storage
- Building construction
- Building costs
- Production over time
- Basic UI feedback

## Scope

MVP 1 includes only the basic wood and construction loop:

Starting Wood → Build Lumberjack  
Lumberjack → Wood  
Wood → Build more buildings

## Starting State

The player starts with:

Wood: 20

Lumberjacks: 0  
Farms: 0  
Storage Buildings: 1

The starting Wood allows the player to build the first Lumberjack and begin the economy.

In MVP 1, the Storage Building represents the player's starting base.

Storage does not have a capacity limit yet.

## Resources

### Wood

Wood is the first basic resource.

Wood is used to construct buildings.

In MVP 1, Wood is produced by Lumberjacks.

## Buildings

### Storage Building

Purpose:

Represents the player's starting base and initial storage.

Rules:

- Starting amount: 1
- Cost: cannot be built in MVP 1
- Input: none
- Output: none
- Storage limit: none in MVP 1

### Lumberjack

Purpose:

Produces Wood over time.

Rules:

- Cost: 10 Wood
- Input: none
- Output: +1 Wood
- Production time: 2 seconds

If multiple Lumberjacks exist, each Lumberjack produces Wood independently.

Examples:

- 1 Lumberjack = +1 Wood every 2 seconds
- 2 Lumberjacks = +2 Wood every 2 seconds
- 3 Lumberjacks = +3 Wood every 2 seconds

### Farm

Purpose:

Represents the first non-wood building that can be constructed with Wood.

In MVP 1, the Farm does not produce anything yet.

This is intentional.

The Farm exists only to prove that Wood can be spent to build other building types.

Rules:

- Cost: 15 Wood
- Input: none
- Output: none in MVP 1
- Production: none in MVP 1

## Player Actions

The player can:

- build a Lumberjack
- build a Farm
- observe Wood increasing over time
- observe Wood decreasing when buildings are built

## UI Requirements

The UI should show:

- current Wood amount
- number of Lumberjacks
- number of Farms
- number of Storage Buildings
- button to build Lumberjack
- button to build Farm

If the player does not have enough Wood, the build button should either:

- be disabled
- show an error message

For MVP 1, disabling the button is preferred because it is simpler and clearer.

## Success Criteria

MVP 1 is successful when:

- the player starts with 20 Wood
- the player starts with 1 Storage Building
- the player can build a Lumberjack for 10 Wood
- the player can build a Farm for 15 Wood
- the player cannot build a building without enough Wood
- each Lumberjack produces Wood over time
- the player can build multiple Lumberjacks
- the player can build multiple Farms
- the UI clearly shows current Wood and building counts
- the UI updates correctly after production and construction

## Out of Scope

The following features are intentionally excluded from MVP 1:

- grain
- flour
- bread
- hunger
- population growth
- workers
- building construction time
- building placement on a map
- storage capacity limits
- tools
- weapons
- soldiers
- combat
- research
- factions
- trading
- neighboring regions
- multiplayer
- saving and loading
- advanced graphics
- animations
- sound
