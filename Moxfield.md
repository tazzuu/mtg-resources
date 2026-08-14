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


# Proxies & Card Sources

Now that you have thoroughly play tested your deck digitally (for free!) its time to start assembling a paper version of the deck, preferably without breaking the bank.

## Buying real cards

You are gonna want to order any preferred real copies of cards from platforms such as [ManaPool](https://manapool.com/), [TCG Player](https://www.tcgplayer.com/), or simply [eBay](https://www.ebay.com/). I find that ManaPool is one of the best sources, because it gives you the option to pay for tracked shipping. This is typically required for orders $50+ USD, but is a boon even for smaller orders in the USA that can easily get lost or delayed by USPS. Tracked shipping is much more reliable and much faster, for both real and proxy cards. TCG Player does not expose these shipping options so it can be unpredictable what type of shipping you get, and so its very common for TCG Player orders shipped untracked via USPS to get lost, rejected, or take 3+ weeks to arrive.

It can still be economical to buy real cards especially for cards that cost less than about $0.50 USD which you may not need quickly, or if you want special versions of cards such as promo stamped or Pre Release date stamped cards.

## Proxy Cards

The section you have all been waiting for. Now its time to start looking at options online for proxy cards. There are many.

In general, there are two types of proxy cards you will encounter:

- custom printed: these are cards which are printed on demand, usually with custom card fronts and non-standard card backs.

- "bootleg" cards: these are cards which are designed to look identical to "real" cards, with original accurate card fronts and standard MTG card backs.

### Custom Printed


#### MPCFill + MPC

- https://mpcfill.com/
  - https://github.com/chilli-axe/mpc-autofill
- https://www.makeplayingcards.com/
- https://www.reddit.com/r/mpcproxies/
- https://www.reddit.com/r/magicproxies/

MPC (Make Playing Cards) is a Chinese vendor that prints custom cards of various types. MPCFill is a software and community project to easily create templates of custom designed MTG cards to be printed with MPC.

This combination of MPC + MPCFill results in high quality cards, albeit with non-standard card fronts and card backs.

The card fronts and arts provided on MPCFill are *not* original card scans. They are typically made by hand by members of the MPCFill Community in an effort to provide "open source" versions of MTG card fronts for use with proxy play. As such, many (if not all) MPCFill card fronts will include deliberate discrepancies compared to the original cards, including things such as different or missing set logos, altered or missing Copyright text, lack of holographic stamps, and other changes to the card frames and typesetting. These cards are always printed with non-standard backs to identify them as proxy cards and not original MTG cards.

MakePlayingCards' product is one of the higher quality ones on the market, especially when ordered with S33 paper, they feel like "real" playing cards and not cheap knock offs. You will want to use the main designer website at https://www.makeplayingcards.com/ to upload your deck (either via pasting in plain-text or, preferred, supplying a public Moxfield etc. deck list URL), then when you are finished custominzing your deck save the .XML file (important!) and run it via command line tool https://github.com/chilli-axe/mpc-autofill/releases/tag to upload the final design straight to the MPC website for checkout. Make sure to use the S33 paper stock for good results.

Note that the cards produced by MPC are printed and shipped from China so take this into account when estimating costs and delivery times. Delivery can take upwards of 14+ days. However the printing quality and final results are above that of other platforms so in general it is worth the wait if you are looking for these custom printed cards. Another note, since they are China-based the company seems to be subject to week-long shut down during certain Chinese holidays, so plan your orders accordingly.

Prices for these cards typically run roughly $0.40/card depending on the size of your order. I would consider this to be a fantastic price considering the quality of the product, a full Commander deck can be printed for roughly $40-50, plus shipping and taxes and fees (tariffs).


#### Self-Printed

There are various resources and communities online that will show you how to print your own proxies at home. The MPC Fill community includes extensive guides on this. Also YouTuber's such as CryCry have detailed guides for this too such as https://www.youtube.com/watch?v=I077so_dEzU

You can also use MPCFill as the basis for self-printing your own proxy cards instead of ordering them from MPC. The following websites help with this;

- https://devprint.taxiera.net/
- https://proxxied.com/

Both of these sites allow you to import or create your decklist for the purpose of printing it yourself, formatted into a PDF with the cards arranged on the page to be cut out easily. If you want to print directly to card stock, you can refer to the previously mentioned self-print guides on the printer type, paper types, and ink types to use. Or if you just need to make quick cheap proxies, you can print these PDFs onto plain office paper using any color printer, cut them out and glue them lightly to basic Land cards and then slide them into deck sleeves and call it a day. This tends to be my preferred option when I am stuck waiting 3+ weeks on "real" cards from TCG Player and just need placeholders while I am filling out the deck.


#### Proxy Printery

- https://proxyprintery.com

A Europe-based custom print proxy website. Notably they are one of the only vendors of holo stamps online, selling their versions of the foil holo stamps that adorn MTG Rare and Mythic Rare cards - the versions they sell include their own wizard mascot logo embedded in the foil stickers in lieu of the WotC mana symbols. The stickers look very good and are a great replacement for foil stickers on any custom cards that may need them. Due to being based in Europe, shipping times to destinations outside of Europe may be very long.

#### MTG Proxy / Printing Proxies

- https://www.mtgproxy.com/
- https://www.printingproxies . com/

Based in the USA, this platform produces low quality custom printed cards for roughly the same price as MPC but with vastly worse quality. While MPC cards look and feel like "real" playing cards, the cards produced by MTG Proxy and its sister websites (there are several, all with the same owner) look and feel like they were printed on a cereal box. The owner of the site has many unprofessional tendencies such as soliciting customers to post positive reviews on his TrustPilot business page which he spams links to everywhere, and publicly berating customers who give negative feedback and ban them from his Discord and deletes their messages and any posts questioning the inferior quality of recieved cards. Additionally, this website hosts and uses stolen card assets from both the MPC Fill community and from Scryfall and other official MTG platforms, and many of the card fronts they provide have the holographic stamp printed on them in plain ink which looks extremely ugly in real life. Interestingly, they sell their own holo stamps to remedy this issue and they are one of the only providers on the internet who sell these. Its not clear how this business persists in the USA in spite of its blatant copyright infringement but regardless its best to not waste your time or money on them when you can get higher quality MPC + MPCFill custom printed proxies for the same price.

#### NotMPC

- https://notmpc.com/

Based in the USA, this company is relatively new (as of time of writing). They seemingly ripped off the website for MPC while marketing themselves as a USA-based alternative to MPC. The business ethics of all this is fishy but they do indeed offer custom printed proxy cards, with the main selling point being that they are based in the USA (West Coast) for slightly faster delivery times than MPC. In practice, China-based MPC usually takes 10-15+ days to deliver, whereas USA-based customers might expect closer to 5-7 days delivery from NotMPC. So there is indeed faster delivery time available from them.

NotMPC's website is surpsingly compatible with MPC Fill; simply upload the .XML file from your MPC Fill deck and it should work on NotMPC. This is very convenient.

In regards to print quality, it is not actually on par with the real MPC, and is surprisingly similar to the quality of MTG Proxy. Not sure if they use the same printing machinery or printing providers or such.

Overall this website is legitimate but given their quality I would typically just wait the extra 5-7 days for delivery from the real MPC instead.

### Replica "Boot Leg" Cards

There are many vendors that supply bootleg MTG cards which are intended to be 1:1 replicas of real cards. Unlike the custom printed proxy vendors who print cards to order, these cards are pre-printed and sold as-is based on available stock. Vendors restock often, and update their stock as new MTG sets are released.

You can find details on several such vendors at the main reddit page

- https://www.reddit.com / r / boot leg mtg

Be sure to check the Wiki for the link to the main Discord, and from the Discord you can find links to individual vendors. Some notable vendors will be highlighted here. This is not a complete list of avaialble vendors just an overview of some.

Note that some vendors are themselves organizing the design and printing of the cards that they sell, while others are only resellers of cards printed by the former. Nearly all non-China based vendors fall into this second category of resellers. Prices for cards from vendors who get their own printings are usually in the range of $1.50 - $3 USD each, while prices from resellers are usually in the range of $3+ each. Foil and non-foil cards are usually the same price, or near identical price. Vendors who are organizing their own printing may or may not sell all their cards as single and may offer packs of pre-selected cards in the range of ~56 cards per pack for a price of roughly $56-65 USD per pack.

#### Black Lotus (BL)

- blacklotuscards . com

Based out of China, this vendor offers a large inventory of cards both as singles and in packs. Previously the most convenient way to order was to find the link to his Google Sheet in the Discord server and then follow the embedded links to his Ali Express pages offering the cards or packs listed. Now there is a dedicated site it seems at blacklotuscards . com . This vendor is notable for having an extensive list of pre-selected card packs which include many MTG staples. They also have sets of speciality foil cards which are very high quality.

#### Underground Sea (Usea)

- agamecardshop . com

Based out of China, this vendor also has a convenient website. If you check their Discord (linked from the main bootletmtg Discord) they also have links to a Google Sheets based decklist importer to help match up cards from your decklist to available inventory. This vendor is also notable for offering many bundles and fixed sets of common cards such as dual lands, and thus is a great place to get low cost sets of duals, shock lands, and other staples that you will need in many decks. After you place an order on the website you will usually get an email within 24hrs with the payment details (they do billing manually for orders placed online).

#### BootlegMage

- bootlegmage . com

A USA based reseller offering a large inventory of cards. Their cards are high quality and this vendor is very reliable however due to popularity the processing and delivery times can be a little lengthy and sometimes unpredictable. This is a good vendor to order cards from for slightly faster delivery than you would get from a China based vendor but be sure to cross check inventory against other vendors because they often run out of stock on popular cards. They frequently update their stock so subscribe to their page for updates. Also they have (had?) a built in deck list importer in their site. Be sure to check their Discord, they are very communicative and offer good service. BootlegMage has been a staple of the community and and frequently offers help online to folks who are order from other vendors as well. Many thanks to him and his team for all their hard work.

#### Tolarian Library / Last Genesis

- lastgenesis . com

A USA based reseller. This one is not part of the Reddit /r/bootlegmtg group and instead has (had) a reddit at https://www.reddit.com/r/CreateMTG/ . This reseller is notable for insanely fast shipping speeds. While most other USA based resellers are delivering cards in about 5-10 business days (sometimes longer), Tolarian Library somehow manages to consistenly deliver within 3-5 business days. Its not uncommon for orders placed on Saturday or Sunday to arrive at your door by Thursday or Friday. The quality of their cards is the same as all other bootleg vendors, and their website includes a deck list importer as well. They have some sort of community-based printing request system in place as well. Overall this is an extremely high quality and reputable vendor for USA-based customers. Note that they recently changed their name and their domain to "Last Genesis". Same vendor with the same high quality cards and same fast shipping.

# Putting it all together

Between the resources described here, we have complete coverage of all the essentail resources needed to prototype, test, and build Magic the Gathering decks, especially for the Commander format.

- start building your decklist with online platforms
- test your decks with digital free simulators
- assemble your paper deck from a mix of vendors to suite your budget and desired card attributes

# References

- ["How to Make Proxies" by JollyCasual](https://moxfield.com/decks/Lk1SbEgVxk6x46FlbuIDDw/primer)