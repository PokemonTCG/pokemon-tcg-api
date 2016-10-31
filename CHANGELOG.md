## 1.6.6 (2016-10-30)
The following sets have been added:
- POP Series 1
- POP Series 2
- POP Series 3
- POP Series 4
- POP Series 5
- POP Series 6
- POP Series 7
- POP Series 8
- POP Series 9
- Wizards Black Star Promos

## 1.6.5 (2016-10-30)
- Added missing set: Base Set 2 (base4).
- Fixed over 250 cards with a supertype of Pokemon that had a missing nationalPokedexNumber.

## 1.6.4 (2016-10-20)
Added the following missing cards:
- Shiny Legends (SL) from Call of Legends.
- Radiant Collection (RC) from Legendary Treasures.
- Secret Rares from BREAKThrough
- Scramble Energy from Deoxys
- Misc. XY Black Star Promos

## 1.6.3 (2016-10-10)
Adds ability to filter on cards that contain a specific field (addresses issue #17).

For example: `https:api.pokemontcg.io/v1/cards?contains=ancientTrait`

## 1.6.2 (2016-09-28)
The __ability__ field now has a __type__ property. The type will either be Pokemon Power, Poke-Power, Poke-Body, or Ability.

Can now filter on the ability type field via the following URL parameter:

- abilityType

Multiple fixes for baby pokemon found in the ecard and neo sets, including updating their supertype to Pokemon, and adding the missing text field about baby pokemon.

## 1.6.1 (2016-09-14)
Can now filter on abilities via the following URL parameters:

- abilityName
- abilityText

Example: `https://api.pokemontcg.io/v1/cards?abilityName=irritating%20pollen`

## 1.6.0 (2016-09-14)
- Minor performance improvements
- Multiple new response headers added:

1. Link: Link headers with prev, last, next, first links (when appropriate)
2. Page-Size: The page size for the request
3. Count: The amount of elements returned
4. Total-Count: The total number of elements (all pages)
5. Ratelimit-Limit: The ratelimit for a given user
6. Ratelimit-Remaining: The number of requests left before the ratelimit is exceeded.

Examples:

```
Link: <https://api.pokemontcg.io/v1/cards?page=82>; rel="last", <https://api.pokemontcg.io/v1/cards?page=2>; rel="next"
Page-Size: 100
Count: 100
Total-Count: 8190
Ratelimit-Limit: 5000
Ratelimit-Remaining: 4999
```

## 1.5.0 (2016-09-05)
All cards with a supertype of Pokemon that were previously missing the "types" field have all been corrected.

New field added: ancientTrait

Sample card with an ancientTrait: https://api.pokemontcg.io/v1/cards/xy5-77

## 1.4.1 (2016-09-01)
Standard Legal update for 2017 rotation.

## 1.4.0 (2016-08-05)
Added Set: Steam Siege

## 1.3.3 (2016-07-28)
Fixes #8 - Incorrect release date for EX - Sandstorm

## 1.3.2 (2016-07-26)
Fixes #2 - XY and BW promo sets added

## 1.3.1 (2016-07-25)
Fixes #7 - incorrect number of cards for set BREAKpoint

## 1.3.0 (2016-07-21)
Added National Pokedex Number to response for cards that feature a pokemon

## 1.2.0 (2016-05-26)
Support for Pipe Delimiters and fixes #3

## 1.1.0 (2016-05-10)
Fixes #1 (Generations Radiant Collection cards missing)

## 1.0.1 (2016-04-22)
Bug fixes:
- filtering on attack cost
- filter on attack damage

## 1.0.0 (2016-04-21)
First Release
