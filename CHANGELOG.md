## 1.14.0 (2017-11-3)
- Crimson Invasion (sm4) added.

## 1.13.1 (2017-10-25)
- Added 'logoUrl' to sets resource.
- Can now query on multiple card ids with the `id` parameter. For example: `https://api.pokemontcg.io/v1/cards?id=xy1-1|xy1-2|xy1-3`

## 1.13.0 (2017-10-19)
- Shining Legends added (sm35)

## 1.12.3 (2017-10-09)
- Additional SMP promos added

## 1.12.2 (2017-09-14)
- Added `ptcgoCode` to sets resource
- Added `symbolUrl` to sets resource

## 1.12.1 (2017-08-07)
Hi-res images for Burning Shadows (sm3) added.

## 1.12.0 (2017-08-05)
Burning Shadows added (sm3)

Please note that secret rares still have to get added, as well as hi-res images. Rarity will also need to be updated for all cards in the set, as Pokemon.com has apparently removed rarity from their webpages for a given card.

## 1.11.0 (2017-07-17)
- Multiple performance enhancements
- Can now filter the sets resource on an exact name
- nationalPokedexNumber query parameter accepts a list (use logical OR)

## 1.10.0 (2017-05-06)
- Guardians Rising added (sm2)

## 1.9.3 (2017-04-06)
- Added `evolvesFrom` field.
- Added missing attacks field for XYP-XY102

## 1.9.2 (2017-03-16)
Bug fix for #46 and #47

## 1.9.1 (2017-02-23)
- SM Black Star Promos Added (smp)

## 1.9.0 (2017-02-20)
Hi-res images added via `imageUrlHiRes` field.

## 1.8.0 (2017-02-03)
- Sun & Moon Released.
- Fixes #37

## 1.7.7 (2016-01-21)
Fixes #35. BW Black Star Promos series is now Black & White instead of BW

## 1.7.6 (2017-01-09)
Fixed the national pokedex number on the following:

- 47 - Parasect
- 141 - Kabutops
- 233 - Porygon2
- 474 - Porygon-Z
- 601 - Klinklang

Also added a missing attack for xyp-XY97.

## 1.7.5 (2017-01-04)
nationalPokedexNumber query parameter now supports a list

## 1.7.4 (2017-01-03)
Fixed naming of EX cards in BW Black Star Promos

Secret rares and misc missing cards have been added for the following sets:
- Arceus
- Delta Species
- Holon Phantoms
- Legend Maker
- Mysterious Treasures
- Plasma Blast
- Platinum
- Rising Rivals
- Stormfront
- Supreme Victors
- Unseen Forces

## 1.7.3 (2017-01-03)
- Can now filter on the expandedLegal parameter.
- XY Black Star Promos standard legal
- BW Black Star Promos not standard legal

## 1.7.2 (2016-12-29)
New field on the Sets resource (`https://api.pokemontcg.io/v1/sets`): expandedLegal

Secret rares and misc missing cards have been added for the following sets:
- Dragons Exalted
- Boundaries Crossed
- Plasma Storm
- Noble Victories
- Dark Explorers
- Plasma Freeze
- Legendary Treasures
- XY
- Flashfire
- Furious Fists
- Roaring Skies
- Ancient Origins
- Breakthrough
- Breakpoint
- Steam Siege

## 1.7.1 (2016-11-14)
Two new query parameters added:
- attackName
- attackText

## 1.7.0 (2016-10-31)
New expansion released - Evolutions (xy12)

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
