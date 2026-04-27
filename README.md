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

### Replica "Boot Leg" Cards

There are many vendors that supply bootleg MTG cards which are intended to be 1:1 replicas of real cards. Unlike the custom printed proxy vendors who print cards to order, these cards are pre-printed and sold as-is based on available stock.

You can find details on several such vendors at the main reddit page

- https://www.reddit.com / r / bootlegmtg

Be sure to check the Wiki for the link to the main Discord, and from the Discord you can find links to individual vendors. Some notable vendors will be highlighted here. This is not a complete list of avaialble vendors just an overview of some.

Note that some vendors are themselves orchestrating the design and printing of the cards that they sell, while others are only resellers of cards printed by the former group. Nearly all non-China based vendors fall into this second category of resellers. Prices for cards from vendors who get their own printings are usually in the range of $1.50 - $3 USD each, while prices from resellers are usually in the range of $3 each. Foil and non-foil cards are usually the same price, or near identical price. Vendors who are organizing their own printing may or may not sell all their cards as single and may offer packs of pre-selected cards in the range of ~56 cards per pack for a price of roughly $56-65 USD per pack.

#### Black Lotus (BL)

Offers a large inventory of cards both as singles and in packs. Previously the most convenient way to order was to find the link to his Google Sheet in the Discord server and then follow the embedded links to his Ali Express pages offering the cards or packs listed. Now there is a dedicated site it seems at https://blacklotuscards . com . This vendor is notable for having an extensive list of pre-selected card packs which include many MTG staples. They also have sets of speciality foil cards which are very high quality.

#### Underground Sea (Usea)

- https://www . agamecardshop . com

Based out of China, this vendor also has a convenient website. If you check their Discord (linked from the main bootletmtg Discord) they also have links to a Google Sheets based decklist importer to help match up cards from your decklist to available inventory. This vendor is also notable for offering many bundles and fixed sets of common cards such as dual lands, and thus is a great place to get low cost sets of duals, shock lands, and other staples that you will need in many decks. After you place an order on the website you will usually get an email within 24hrs with the payment details (they do billing manually for orders placed online).

#### BootletMage

- https://bootlegmage . com

A USA based reseller offering a large inventory of cards. Their cards are high quality and this vendor is very reliable however due to popularity the processing and delivery times can be a little lengthy and sometimes unpredicatble. This is a good vendor to order cards from for slightly faster delivery than you would get from a China based vendor but be sure to cross check inventory against other vendors because they run out of stock often on popular cards. They frequently update their stock so subscribe to their page for updates. Also they have (had?) a built in deck list importer in their site. Be sure to check their Discord, they are very communicative and offer good service.

#### Tolarian Library

- https://tolarianlibrary . com

A USA based reseller. This one is not part of the Reddit /r/bootlegmtg group and instead has a reddit at https://www.reddit.com/r/CreateMTG/ . This reseller is notable for insanely fast shipping speeds. While most other USA based resellers are delivering cards in about 5-10 business days (sometimes longer), Tolarian Library somehow manages to consistenly deliver within 3-5 business days. Its not uncommon for orders placed on Saturday or Sunday to arrive at your door by Thursday or Friday. The quality of their cards is the same as all other bootleg vendors, and their website includes a deck list importer as well. They have some sort of community-based printing request system in place as well. Overall this is an extremely high quality and reputable vendor for USA-based customers.
