# MTG Resources

Resources guide for Magic the Gathering

# Card & Deck Resources

## Card Databases

### Scryfall

- https://scryfall.com/

Online database of all the MTG cards in existence. Includes an API and bulk data downloads which are useful for developers

### Gatherer

- https://gatherer.wizards.com/

The official WotC card database

## Deck Builders

### Moxfield

- https://moxfield.com/

Super high quality platform to build MTG decks and share them online.

### Archidekt

- https://archidekt.com/

Another high quality deck building website.

# Digital Play Platforms

### Rules Engine Platforms

Platforms with a built in rules engine allow you to play MTG like any other videogame. This means that the game platform enforces card rules and effects for you, so you dont have to "fake it" with tabletop simulators.

#### Card Forge

- https://github.com/Card-Forge/forge

Play against AI opponents here. Also includes single player Campaign modes.

#### X-Mage

- https://github.com/magefree/mage

Play online against other players here

### Tabletop Simulators

These are bare bones platforms that literally just simulate a table and you have to put your digital cards on them and run the game yourself like you would IRL with paper cards. There are a million of these platforms and overall they are all pretty lame and not worth your time but I will include some here for completeness sake.

#### Spelltable

- https://spelltable.wizards.com/

Use a webcam to stream a video feed of your home kitchen table with your cards on it and play against other players who are also streaming video feeds of their kitchen tables. Note that most all players use potato cameras so you likely wont be able to clearly see what cards other players are using. WotC bought this platform at the beginning of COVID and proceeded to never update it. Thanks, Wizards.

#### Cockatrice

- https://cockatrice.github.io/

Plays multiple different games it seems, because again it is just a simulator for your kitchen table with cards on it and does not actually have a rules engine.

#### Tabletop Simulator

- read about it here https://draftsim.com/tabletop-simulator-mtg/

You can pay $20 to have a virtual version of your kitchen table

#### Others

There are a million other tabletop simulators you can find online, try them if you want. Seems like a new one pops up every other month.

### WotC Ditigal Platforms

you can play the official digital versions of Magic on [Arena](https://magic.wizards.com/en/mtgarena) and [MTG Online](https://www.mtgo.com/home) though these both have serious issues and downsides such as limited OS compatibility and locked-in cards as digital objects meaning you cannot just load up any deck you want you have to actually pay money for digital cards to play with. Yuck.

# Paper Cards

## Buying real cards

If you are gonna pay money for real cards the best places to shop are [TCG Player](https://www.tcgplayer.com/) for the vast majority of cards, and occasionally [eBay](https://www.ebay.com/) for one-off or special cases or niche cards. For example the ["racist cards"](https://magic.wizards.com/en/news/announcements/depictions-racism-magic-2020-06-10) cannot easily be found on TCG Player or other online card stores but are easy to find on eBay. You can also find dealers on eBay specializing in things like vintage cards more easily than on TCG Player.

## Proxy Cards

In general there are two types of proxy cards you will encounter;

- custom printed proxies: by far the most commonly used, these are websites that will print to order a list of your desired cards and usually have multiple options for which art and card front designs to use. These almost always have non-standard card backs so its easy to tell from the back of the card that its a proxy.

- "bootleg" proxy cards: these are cards designed to be 1:1 replicas of "real" Magic cards and look identical to official cards. Note that the term "real MTG cards" itself is pretty ambiguous since WotC does not even print their own cards and instead offloads printing to multiple third party contractors of inconsistent print quality, so the notion that these cards are "less real" is itself kinda iffy. Regardless these cards come in a range of qualities but these days most are indistinguishable from real cards unless you use a magnifying glass to examine them.

Most proxy card platforms have robust online communities backing them, so be sure to look for their associated Discord and Reddit groups for more details and resources.

### Custom Print

#### MPCFill + MPC

- https://mpcfill.com/
  - https://github.com/chilli-axe/mpc-autofill
- https://www.makeplayingcards.com/
- https://www.reddit.com/r/mpcproxies/
- https://www.reddit.com/r/magicproxies/

This is a combination of two resources; MPC (MakePlayingCards.com) is a website for a printing company based out of China who produce extremely high quality custom printed playing cards. MPCFill is an open source community & web based design platform used to design free open source third party card fronts and card backs to use for creating proxy MTG cards with MPC.

Its important to note that the card fronts shown at MPCFill are *not* the original card fronts. Instead they are custom designed by community members using some of the official MTG artwork and several different card-frame and border templating engines. These cards are always printed with non-standard backs as well.

You will want to use the main designer website at https://www.makeplayingcards.com/ to upload your deck (either via pasting in plain-text or, preferred, supplying a public Moxfield etc. deck list URL), then when you are finished custominzing your deck save the .XML file (important!) and run it via command line tool https://github.com/chilli-axe/mpc-autofill/releases/tag to upload the final design straight to the MPC website for checkout. Make sure to use the S33 paper stock for good results.

Note that the cards produced by MPC are printed and shipped from China so take this into account when estimating costs and delivery times. Delivery can take upwards of 14+ days. However the printing quality and final results are above that of other platforms so in general it is worth the wait if you are looking for these custom printed cards. Another note, since they are China-based the company seems to be subject to week-long shut down during certain Chinese holidays, so plan your orders accordingly.

#### MTG Proxy / Printing Proxies

- https://www.mtgproxy.com/
- https://www.printingproxies.com/

Based in the USA, this platform produces low quality custom printed cards for roughly the same price as MPC but with vastly worse quality. While MPC cards look and feel like "real" playing cards, the cards produced by MTG Proxy and its sister websites (there are several, all with the same owner) look and feel like they were printed on a cereal box. The owner of the site has many unprofessional tendencies such as soliciting customers to post positive reviews on his TrustPilot business page which he spams links to everywhere, and publicly berates customers who give negative feedback and bans them from his Discord and deletes their messages and any posts questioning the inferior quality of recieved cards. Additionally, this website hosts and uses stolen card assets from both the MPC Fill community and from Scryfall and other official MTG platforms, and many of the card fronts they provide have the holographic stamp printed on them in plain ink which looks extremely ugly in real life. Interestingly, they sell their own holo stamps to remedy this issue and they are one of the only providers on the internet who sell these. Its not clear how this business persists in the USA in spite of its blatant copyright infringement but regardless its best to not waste your time or money on them when you can get higher quality MPC + MPCFill custom printed proxies for the same price.

#### NotMPC

- https://notmpc.com/

Based in the USA, this company is relatively new (as of time of writing) and was flagged as a "scam" but actually is a legitimate business. They seeemingly ripped off the website for MPC while marketing themselves as a USA-based alternative to MPC. The business ethics of all this is fishy but they do indeed offer custom printed proxy cards, with the main selling point being that they are based in the USA (West Coast) for slightly faster delivery times than MPC. In practice, MPC usually takes 10-15+ days to deliver, whereas USA-based customers might expect closer to 5-7 days delivery from NotMPC.

Since they ripped off the MPC website, NotMPC's website is surpsingly compatible with MPC Fill; simply upload the .XML file from your MPC Fill deck and it should work on NotMPC. This is very convenient.

In regards to print quality, it is not actually on par with the real MPC, and is surprisingly similar to the quality of MTG Proxy. Not sure if they use the same printing machinery or printing providers or such.

Overall this website is legitimate but given their quality I would typically just wait the extra 5-7 days for delivery from the real MPC instead.

#### Proxy Printery

- https://proxyprintery.com

A Europe-based custom print proxy website. Notably they are one of the only vendors of holo stamps online, selling their one versions of the foil holo stamps that adorn MTG Rare and Mythic Rare cards - the versions they sell include their own wizard mascot logo embedded in the foil stickers in lieue of the WotC mana symbols. The stickers look very good and are a great replacement for foil stickers on any custom cards that may need them. Due to being based in Europe, shipping times to destinations outside of Europe may be very long.