# MTG Proxy & Playtest Resource Guide

A complete guide on the best resources to use for building Commander decks. This end-to-end guide covers the resources used to get started prototyping and play testing your deck digitally, and then turn it into a paper deck in a budget friendly manner via proxy cards.

---

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

Start using one of these websites to build your deck list.

#### Moxfield

- https://moxfield.com/

Super high quality platform to build MTG decks and share them online.

#### Archidekt

- https://archidekt.com/

Another high quality deck building website.

#### Others

There are many other deck building websites out there, you can Google search for them.

### Card Cataloging

Once you have accumulated 1000's of paper cards, you need to start tracking your collection digitally so that you can easily reference it and look up which cards you own. These apps typically include the ability to scan your card with your phone's camera to identify it and add it to a collection in your account. You can usually export the collection in various formats for usage with different websites.

#### Shiny

- https://www.getshiny.io/

You can use the Shiny app to scan and catalogue your paper cards. The Pro version allows for .csv and .json export of your collection.

#### ManaBox

- https://manabox.app/

Another very popular app for building and maintaining your digital card catalogue.

## Digital Play Platforms

Once you have built a prototype of your deck, you will want to take it for real play tests in order to see how it performs. There are two basic types of platforms for this: rules engines, and table top simulators.

### Rules Engine Platforms

Platforms with a built in rules engine allow you to play MTG as if it was any other videogame. This means that the game enforces card rules and effects for you, so you never miss a trigger or botch a card interaction. Rules Engines allow you to play MTG "for real" the way its meant to be played, instead of faking it with tabletop simulators.

#### Card Forge

- https://github.com/Card-Forge/forge

Play against AI opponents here. Also includes single player Campaign modes.

Card Forge lets you easily import your own decks to play with. You can play against included decks, and you can download some top decks from Moxfield and Archidekt to load into Forge here: https://github.com/tazzuu/mtg-decks

Card Forge is by far the best platform for offline Rules Engine play. You can load it up with 3x AI opponents, giving each of them a Commander deck, and you can play "real" Commander against the AI's. While the behavior of the AI opponents is not always true to how real life human players would play, you can get a very strong sense of how your deck performs.

Using Card Forge is critical for deck building, because it lets you run play tests of your prototype deck over and over again very quickly and easily for FREE. You can load up the deck list you made in Moxfield or other sources into the game by using [mtgconv](https://github.com/tazzuu/mtgconv) to produce a properly formatted .dck deck list file to import into the game.

Once your deck can consistently win against the AI in Card Forge, its usually safe to start piecing it together in paper to try out at the LGS for further testing and review.

Note that Card Forge runs on Windows, macOS, Android, and Linux. Notably absent is iOS. My suggestion, is to get a "cheap" Android tablet in the ~11" size range that has at least 8GB RAM (and a kick-stand or folio-stand included), and use that as your primary Forge platform. You can also use Android phones with great success. Performance on the game is generally good unless you or an opponent accumulates 10's of Tokens, in which case the game can suffer severe lag (it has to calculate possible interactions between every card and every token, for every game action), so try to avoid playing [[Scute Swarm]] and similar uncontrollable Token-makers. Also notes that the game tends to crash if a single game object or creature accumulates more than 1 billion counters. So avoid that as well (looking at you [[Mossborn Hydra]]).

#### X-Mage

- https://github.com/magefree/mage

Play online against other players here.

Personally I have never actually used it but this one is recommended for online play against human opponents. While Card Forge does have an online play client, I am not sure if its popular, meanwhile X-Mage does seem to have a more active online player base.

### Tabletop Simulators

These are bare bones platforms that literally just simulate a table and you have to put your digital cards on them and run the game yourself like you would IRL with paper cards. There are a million of these platforms and overall they are all pretty lame and not worth your time but I will include some here for completeness sake.

#### Spelltable

- https://spelltable.wizards.com/

Use a webcam to stream a video feed of your home kitchen table with your cards on it and play against other players who are also streaming video feeds of their kitchen tables. Note that most all players use potato cameras (or, the video stream you get of their table is usually of potato-quality) so you likely wont be able to clearly see what cards other players are using. WotC bought this platform at the beginning of COVID and proceeded to never update it. Thanks, Wizards.

#### Cockatrice

- https://cockatrice.github.io/

Plays multiple different games it seems, because again it is just a simulator for your kitchen table with cards on it and does not actually have a rules engine.

#### Tabletop Simulator

- read about it here https://draftsim.com/tabletop-simulator-mtg/

You can pay $20 to have a virtual version of your kitchen table. Strong pass. Or play it, if you like.

#### Others

There are a million other tabletop simulators you can find online, try them if you want. Seems like a new one pops up every other month.

### WotC Ditigal Platforms

you can play the official digital versions of Magic on [Arena](https://magic.wizards.com/en/mtgarena) and [MTG Online](https://www.mtgo.com/home) though these both have serious issues and downsides such as limited OS compatibility and locked-in cards as digital objects meaning you cannot just load up any deck you want you have to actually pay money for digital cards to play with. Yuck.








# References

- ["How to Make Proxies" by JollyCasual](https://moxfield.com/decks/Lk1SbEgVxk6x46FlbuIDDw/primer)