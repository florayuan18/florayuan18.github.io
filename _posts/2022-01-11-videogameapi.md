---
layout: post
title: Video Game API
subtitle: RAWG API
cover-img: /assets/img/videogamebackground.jpg
thumbnail-img: /assets/img/rawgapi.png
share-img: /assets/img/videogamebackground.jpg
gh-repo: daattali/beautiful-jekyll
tags: [api, video game]
comments: true

---
**Goals**
- Retrieve the newest and hottest games!
- Displays game icons and summaries for user convenience
- Implements search bar

**Potential Features**
- Display user ratings for each game
- Recommendations for new games based on user trends/preferences

### Updates

{: .box-note}
**01/12/22:** Search Bar has been implemented.

Example of Valorant Search:

![Valorant](/assets/img/valorantsearch.png)

Sample Code for API:

```javascript
public class SearchCTRL {
  @GetMapping("/search")
  public String RawgAPI(@RequestParam(name="search", required=true, defaultValue= "") String search, Model model) throws IOException, InterruptedException, ParseException, JSONException {

  String KEY = "42771867b81b456496770e0c1c15d4f2";
  String url = "https://api.rawg.io/api/games?key=" + KEY + "&search=" + search;
```



