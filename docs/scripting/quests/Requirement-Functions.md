# Requirement Functions
 Requirements are things that must be met for the player to receive a quest or proceed in a dialogue.
 You can combine requirements with logic using the and, or, and not requirements. These should allow you
 to create any kind of requirement.

## hasQuestRequirement

A requirement for a player to have a quest.

### Signature:
```js
Requirement hasQuestRequirement(String questId)
```
### Arguments:

**questId**: The quest's ID.

## levelRequirement

A requirement for the player to be a certain level (experience).

### Signature:
```js
Requirement levelRequirement(Integer level)
```
### Arguments:

**level**: The level, as an integer.

## orRequirement

A requirement for the player to have either requirement, or both.

### Signature:
```js
Requirement orRequirement(Requirement requirement, Requirement requirement2)
```

## notRequirement

A requirement for the player _not_ to have a requirement.

### Signature:
```js
Requirement notRequirement(Requirement requirement)
```
### Arguments:

**requirement**: The requirement for them not to have.

## reachedStageRequirement

A requirement for the player to have reached a specific stage of a quest. Only works with
 staged quests.

### Signature:
```js
Requirement reachedStageRequirement(String questId, Integer stage)
```
### Arguments:

**questId**: The ID of the quest.

**stage**: The index of the stage to check for.

## moneyRequirement

A requirement for the player to have a certain amount of money.

### Signature:
```js
Requirement moneyRequirement(Double amount, Currency currency)
```
### Arguments:

**amount**:   The amount of money.

**currency**: The money's currency.

## andRequirement

A requirement that requires two requirements to be met.

### Signature:
```js
Requirement andRequirement(Requirement requirement, Requirement requirement2)
```
### Arguments:

**requirement**:  The first requirement.

**requirement2**: The second requirement.

## turnedInQuestRequirement

A requirement for having turned in a quest.

### Signature:
```js
Requirement turnedInQuestRequirement(String questId)
```
### Arguments:

**questId**: The quest's ID.

