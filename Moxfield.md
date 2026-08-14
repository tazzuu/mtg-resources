# MTG Proxy & Playtest Resource Guide

A complete guide on the best resources to use for building Commander decks. This end-to-end guide covers the resources used to get started prototyping and play testing your deck digitally, and then turn it into a paper deck in a budget friendly manner via proxy cards.

## Card & Deck Resources

These websites will be your best sources for details about cards

### Card Databases

#### EDHRec

- https://edhrec.com/

The starting point for most Commander deck building. This website lists the top Commanders in play and the top cards that are used by them. This is a fantastic reference point to get a sense of what is currently popular in the game. Its also a great refernce to check up on any cards you might have missed for your given Commander. If you want to get ideas on what other strong commanders are out there and how decks might be built around them, this is the site for you. When coming up with ideas for new decks, if I didnt start with a pre-con deck, then I am frequently browsing the Commanders listed on this site for various color combinations to see what seems interesting to play. Make sure to check back repeatedly during your deck building because I often find that early in deck building I may have pre-maturely disregarded cards listed for a given Commander so its helpful to re-review the EDHRec page for the Commanders' top cards to help surface things I may have missed.

#### Scryfall

- https://scryfall.com/

Online database of all the MTG cards in existence, including all printings of all cards. Includes an API and bulk data downloads which are useful for developers. Most importantly, it has an extremely robust Search interface, allowing you to drill down to all the cards that match given criteria.

Example: all the non-creature spells in Blue / Black / White colors (color identity) that mention "Lifelink", sorted by increasing mana value

```
oracle:lifelink (game:paper) prefer:oldest -type:creature -type:land ci:uwb order:cmc dir:asc
```

https://scryfall.com/search?q=oracle%3Alifelink+%28game%3Apaper%29+prefer%3Aoldest+-type%3Acreature+-type%3Aland+ci%3Auwb+order%3Acmc+dir%3Aasc&unique=cards&as=grid&order=name

If you are a developer make sure to review the API and Bulk Data Download pages

- https://scryfall.com/docs/api

- https://scryfall.com/docs/api/bulk-data

Its particularly helpful that Scryfall makes available various JSON files which include the Oracle text and description for every card, allowing you to do card searchs via your custom programs offline.

#### Gatherer

- https://gatherer.wizards.com/

The official WotC card database. Good for cross-referencing somethings but in general Scryfall ends up being most useful.

### Deck Builders

#### Moxfield

- https://moxfield.com/

Super high quality platform to build MTG decks and share them online.

#### Archidekt

- https://archidekt.com/

Another high quality deck building website.





# References

- ["How to Make Proxies" by JollyCasual](https://moxfield.com/decks/Lk1SbEgVxk6x46FlbuIDDw/primer)