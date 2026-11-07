# CRUX

An outdoor rock climbing companion: discover climbs, find beta, log sessions, track projects and climb with your crew.

This is an interactive prototype built as a single HTML page. It runs entirely in the browser and stores its data in `localStorage` on your device.

## Run it

Open `index.html` in a browser, or serve the folder:

```
python3 -m http.server 8000
```

Then visit http://localhost:8000. The photos are loaded from the `img/` folder, so keep it next to `index.html`.

## What's in it

- **Home:** your most recent project and a photo-led feed from your friends.
- **Log a session:** the one place to record climbing. Add climbs as Sent (flash, onsight, redpoint, repeat) or Attempted, with optional notes, photos and conditions per climb. Attempts can be saved to My Projects.
- **Projects:** Active, Completed and Wishlist. Project progress, completion and history are reconciled from your logged sessions.
- **Beta:** snap or upload a photo of a climb, add where it is and its name, and get a match plus a suggested beta overlay (hand and foot markers, arrows, start and finish, move timeline).
- **Profile:** progress stats, grade chart, a calendar of logged days, and friends.
- **Friends:** a mutual friends system with requests that must be accepted, search, suggestions and invites.

## Notes

- Photo identification and AI-suggested beta use Claude through the claude.ai artifact runtime (`window.claude`). Outside claude.ai these features show a clear "not available" message, and matching falls back to the location and name you enter.
- People, sessions, friend activity and the example beta annotations are sample data. The climbs and climbing areas are real.
- Invite links (`crux.app/invite/...`) are placeholders.

## Photo credits

Route and area photos are from [Wikimedia Commons](https://commons.wikimedia.org/), cropped and resized for this app. Each image keeps its original license. Adapted versions of CC BY-SA images are shared under the same license.

| File | Original | Author | License |
|---|---|---|---|
| `img/babyface.jpg` | [Hueco Tanks - Babyface v7.jpg](https://commons.wikimedia.org/wiki/File:Hueco_Tanks_-_Babyface_v7.jpg) | Dana Le | CC BY 2.0 |
| `img/buttermilks.jpg` | [Bouldering at The Buttermilks.jpg](https://commons.wikimedia.org/wiki/File:Bouldering_at_The_Buttermilks.jpg) | Mark Doliner | CC BY 2.0 |
| `img/cardiopalma.jpg` | [Fabio Palma, Cardiopalma, 7c, Kalymnos.jpg](https://commons.wikimedia.org/wiki/File:Fabio_Palma%2C_Cardiopalma%2C_7c%2C_Kalymnos.jpg) | Ultimouomo | CC BY-SA 4.0 |
| `img/convicted.jpg` | [Red River Gorge - Motherlode - Convicted 2.jpg](https://commons.wikimedia.org/wiki/File:Red_River_Gorge_-_Motherlode_-_Convicted_2.jpg) | Jarek Tuszyński | CC BY 3.0 |
| `img/governor.jpg` | [Hueco Tanks - The Governor.jpg](https://commons.wikimedia.org/wiki/File:Hueco_Tanks_-_The_Governor.jpg) | Dana Le | CC BY 2.0 |
| `img/grandpa.jpg` | [Buttermilks (16686546026).jpg](https://commons.wikimedia.org/wiki/File:Buttermilks_%2816686546026%29.jpg) | Kunstee | CC BY 2.0 |
| `img/happy.jpg` | [Happy Sky, Happy Boulders.jpg](https://commons.wikimedia.org/wiki/File:Happy_Sky%2C_Happy_Boulders.jpg) | Mark Doliner | CC BY-SA 2.0 |
| `img/heroroof.jpg` | [Hero Roof, V0 Buttermilks (16712472825).jpg](https://commons.wikimedia.org/wiki/File:Hero_Roof%2C_V0_Buttermilks_%2816712472825%29.jpg) | Kunstee | CC BY 2.0 |
| `img/hpd.jpg` | [High Plains Drifter (V7) - Buttermilks - Bishop, California.jpg](https://commons.wikimedia.org/wiki/File:High_Plains_Drifter_%28V7%29_-_Buttermilks_-_Bishop%2C_California.jpg) | Maria Ly | CC BY-SA 2.0 |
| `img/hueco.jpg` | [Hueco Tanks Bouldering.jpg](https://commons.wikimedia.org/wiki/File:Hueco_Tanks_Bouldering.jpg) | Surfsupusa | Public domain |
| `img/loaded.jpg` | [Loaded with Power V10 Hueco Tanks Texas.jpg](https://commons.wikimedia.org/wiki/File:Loaded_with_Power_V10_Hueco_Tanks_Texas.jpg) | Dana Rader | CC BY 2.0 |
| `img/midnight.jpg` | [Midnight Lightning yosemite.jpg](https://commons.wikimedia.org/wiki/File:Midnight_Lightning_yosemite.jpg) | Mark Donoher | CC BY 2.0 |
| `img/midnight2.jpg` | [Midnight Lightning Columbia Boulder.jpg](https://commons.wikimedia.org/wiki/File:Midnight_Lightning_Columbia_Boulder.jpg) | Andrew Davidoff | CC BY-SA 2.0 |
| `img/midnight3.jpg` | [Midnight Lighting Camp 4.jpg](https://commons.wikimedia.org/wiki/File:Midnight_Lighting_Camp_4.jpg) | fran-42 | CC BY-SA 2.0 |
| `img/midnight4.jpg` | [Midnight Lightning erased on 5-28-19.jpg](https://commons.wikimedia.org/wiki/File:Midnight_Lightning_erased_on_5-28-19.jpg) | Yosemite2 | CC BY-SA 4.0 |
| `img/pureimag.jpg` | [Sasha DiGiulian - Pure Imagination 2011 - 1.jpg](https://commons.wikimedia.org/wiki/File:Sasha_DiGiulian_-_Pure_Imagination_2011_-_1.jpg) | EpicTVAdventure | CC BY 3.0 |
| `img/silverchair.jpg` | [Bouldering Hollow Mountain Cave 1.jpg](https://commons.wikimedia.org/wiki/File:Bouldering_Hollow_Mountain_Cave_1.jpg) | Simon Li | CC BY 2.0 |
| `img/snl.jpg` | [Saturday Night Live V4.jpg](https://commons.wikimedia.org/wiki/File:Saturday_Night_Live_V4.jpg) | ben klocek | CC BY 2.0 |
| `img/stemgem.jpg` | [Joshua Tree bouldering - Stem Gem 4.jpg](https://commons.wikimedia.org/wiki/File:Joshua_Tree_bouldering_-_Stem_Gem_4.jpg) | Jarek Tuszyński | CC BY-SA 3.0 |
| `img/stemgem2.jpg` | [Joshua Tree bouldering - Stem Gem 1.jpg](https://commons.wikimedia.org/wiki/File:Joshua_Tree_bouldering_-_Stem_Gem_1.jpg) | Jarek Tuszyński | CC BY-SA 3.0 |
| `img/teatime.jpg` | [Tea Time 7C+ Rocklands South Africa.jpg](https://commons.wikimedia.org/wiki/File:Tea_Time_7C%2B_Rocklands_South_Africa.jpg) | Dana Rader | CC BY 2.0 |
