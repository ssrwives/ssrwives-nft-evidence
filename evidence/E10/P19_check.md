# P19 check: Steam record of NFT holders receiving a free copy, key or other perk
Checked 2026-10-18 17:46–17:50 PT (2026-10-19 00:46–00:50Z), logged out and read-only.
Promise under test (from casefile; this is not a Steam source): @HedProtag on X, 2023-08-29, said NFT holders would "get the game completely for free at launch", plus an early demo.

## Conclusion
**I found no Steam record of SSR Wives NFT holders getting a free copy, a free key, a giveaway or any other holder perk.** That covers app 2880000, the relisted app 4553340 and the demo 4554620, across every captured store version, the news and events feeds, and the discussion boards.
- No Steam page mentions holders, whitelists, wallets, verification, redeem codes or key giveaways.
- **The full game hasn't launched on Steam.** App 4553340 reads "Release Date: Coming soon" ("This game is not yet available on Steam"), appdetails shows `coming_soon: true` with no price, and there are 0 reviews.
- The only build ever released is the demo, app 4554620. It's free for every Steam user, with release date "Mar 31, 2026". Nothing on Steam ties it to holders.
- On app 2880000 the earlier demo was public; the dev said on 2025-11-29 "I made the Beta version of the demo public!". There's no holder-only access anywhere.
- The only Steam statements about NFTs at all are developer denials and one sarcastic reply (below).

## Current state (2026-10-18)
| app | store | appdetails | news (ISteamNews) | events API | reviews |
|---|---|---|---|---|---|
| 4553340, the full game | https://store.steampowered.com/app/4553340/: "Release Date: Coming soon"; Developer and Publisher both Hen Studios; offers "Download SSR Wives: The Murder Of My Winter Crush Demo"; no price | `success:true`, `release_date: {coming_soon: true, date: "Coming soon"}`, `is_free: false`, no `price_overview`, `package_groups: []`; demos: 4554620. No change from the 2026-10-17 capture | count 0 | 0 events | 0 ("No user reviews") |
| 4554620, the demo | /app/4554620/ redirects to /app/4553340 | `type: demo`, `release_date: {coming_soon: false, date: "Mar 31, 2026"}`, `is_free: true`, fullgame 4553340 | count 0 | 0 | 0 |
| 2880000, the original | Redirects to the Steam home page | `{"2880000":{"success":false}}` | 4 items; the last is 2025-07-23 ("Demo Disc Super Update! (July 2025)") | 3 | 0 |

Store news pages /news/app/4553340 and /news/app/4554620 have no posts. The community announcement pages /games/4553340/announcements and /games/4554620/announcements also have no posts.

- **Discussions on 4553340:** one subforum (General, /discussions/0/) holding a single topic, 801217828677077903, "Due to trolls posting will be disabled". Gilgamesh [developer] started it 2026-04-01 18:22 PT. It has 9 comments, the last on 2026-09-18, and none of them is about holder perks, keys or free copies.
- **Discussions on 4554620:** the community URLs (/discussions/, /guides/, the hub) redirect to the store page for 4553340, so the demo has no board of its own.
- **Guides:** 0 items on 4553340 and on 2880000.
- **FAQ:** the 4553340 store page has no FAQ section.

## What I searched
**Terms**, matched as case-insensitive whole words: holder(s), free, key(s), copy/copies, giveaway(s), whitelist(ed), WL, wallet(s), verify/verified/verification, NFT(s), mint(ed/ing), OpenSea, launch(ed/es/ing), redeem(ed/ing), code(s).

**Sources:**
1. **All board posts:** 699 posts in total, being the 689 posts from all 129 topics on app 2880000 (crawled 2026-10-17, raw/all_posts.json) plus the 4553340 thread (OP and 9 comments, fetched 2026-10-18). Combined file: p19/all_posts_incl_4553340.json.
2. **Store versions of 2880000:** Wayback captures 20240522092051, 20240816053320, 20241006133136, 20250323035045, 20250429025056, 20250527000525, 20250611192035, 20250726022323, 20250813001355 and 20250909143819 (read via WebFetch; transcribed in raw/wayback/webfetch_store_snapshot_fields.md), plus ledger's raw HTML from 2025-11-16.
3. **Store pages and appdetails:** 4553340 on 2026-10-17 and 2026-10-18; 4554620 and 2880000 on 2026-10-18.
4. **News and events:** news API and events API for all three apps, the store news pages, and the community announcement pages.
5. **Guides, hubs and reviews APIs** for all three apps.
6. **hedprotag's Steam profile.**

Exact URLs are in p19/items.tsv and p19/needs_archive.txt.

**Excluded as noise:**
- "key"/"keys" used for in-game items ("find keys to open locked rooms", "key areas").
- "Copy" from the Steam widget text ("Copy and paste the HTML").
- "Free" from Steam's own navigation and other games' listings.
- "launched" in "since we launched", which refers to the store page; see below.

## Hits
Developer posts, all with the Steam [developer] badge and no edit markers. The full-page PNGs and raw HTML are in p19/.
1. **hedprotag** (https://steamcommunity.com/id/hedprotag), 2025-06-23 17:18 PT, "Demo Flop": https://steamcommunity.com/app/2880000/discussions/0/664957644709066572/#c591774962691373396
   > "Developer here:\nThere are no NFTs Tied to SSR Wives: The Murder Of My Winter Crush."
2. **hedprotag**, 2025-06-23 17:19 PT, "why nft?": https://steamcommunity.com/app/2880000/discussions/0/664957644709060789/#c591774962691373423
   > Same text as hit 1.
3. **hedprotag**, 2025-11-29 17:15 PT, "so the game is dead, right?" (page 3): https://steamcommunity.com/app/2880000/discussions/0/685237821971197677/#c684113073641982428
   > "The game won't have any NFT integration."
4. **myfemdomfantasy** (https://steamcommunity.com/profiles/76561198116923409), 2025-06-14 12:26 PT, "Not Recommended": https://steamcommunity.com/app/2880000/discussions/0/664957644709044750/#c664957644709048992
   > "…And YES it IS an NFT scam where every piece of ammo in game will have to be an NFT you buy for 30 dollars PER BULLET…"

   This reads as sarcasm in a reply to a negative thread. It makes no holder offer.
5. **Gilgamesh** (https://steamcommunity.com/profiles/76561199659748947), app 4553340, 2026-04-01 18:37 PT: https://steamcommunity.com/app/4553340/discussions/0/801217828677077903/#c801217828677078568
   > "We’ve gotten hundreds of wishlists since we launched!"

   "Launched" here refers to the store page or demo. It says nothing about holders or free copies.

Non-developer posts:
- **Matches for "holder" (3 posts):** all use it in the sense of copyright/IP holder, not NFT holder.
  - https://steamcommunity.com/app/2880000/discussions/0/684112827030472316/#c684112827030585795 (2025-11-27)
  - https://steamcommunity.com/app/2880000/discussions/0/682987562005020593/#c803469628489722918 (2026-04-02)
  - https://steamcommunity.com/app/2880000/discussions/0/682987562005020593/#c803470345661111041 (2026-04-09)

  These posts name a private person; I haven't quoted them here.
- **Other NFT posts:** the remaining non-dev NFT mentions ("why nft?" and similar) ask about NFTs. None of them reports getting a free copy, a key or a holder perk.
- **Zero hits anywhere on Steam:** whitelist, WL, wallet, verify/verification, redeem, giveaway, mint, holder demo, free key, free copy.

## Captures
- 24 items (PNG, raw file, sha256), indexed in `/workspace/casefile/evidence/steamtrail/p19/preservation_index_p19.csv` and mirrored in `/workspace/steamtrail/p19/`.
- archive.ph: not submitted; the URLs are in needs_archive.txt for browser submission.
- Wayback: not attempted, because web.archive.org is unreachable from the box.
