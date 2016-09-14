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
