#DPTV

Repo to handle technical issues with [Denver Post TV](http://dptv.denverpost.com) and [The Sports Show](http://sportsshow.denverpost.com/).

## DPTV Production Help
### How to import videos by hand
In the wp-admin of DPTV and Sports Show is a page called Ooyala Debug (Settings -> Ooyala Debug).

On that page is a form, and if you paste in the ooyala video id for the video you're looking for, it will import it (unless it's already in the system, then it just lets you know it's already in the system).

* [Here's that page for DPTV](http://dptv.denverpost.com/wp-admin/options-general.php?page=ooyala-debug)
* [And for the Sports Show](http://sportsshow.denverpost.com/wp-admin/options-general.php?page=ooyala-debug)

Once a video is imported it will be in draft mode, and you will need to add a category to it.

## Useful links

Ooyala API web interface: https://api.ooyala.com/docs/api_scratchpad

Ooyala video editor: http://backlot.ooyala.com/backlot/web

Ooyala player editor -- the place where you add or remove tabs from the bottom row of the player (aka themebuilder): https://themebuilder.ooyala.com/

Ooyala Support: https://ooyalacommunity.force.com/apex/Home

Documentation for Backlot external publisihing XML template language: http://support.ooyala.com/documentation/reference/fms.html

Template tag date filter syntax: http://docs.shopify.com/themes/liquid-documentation/filters/additional-filters#date

### HTML 5 Player Reference
* [Customize the UI](http://support.ooyala.com/developers/documentation/concepts/player_v3_dev_customui.html)
* [Javascript API reference](http://support.ooyala.com/developers/documentation/concepts/book_api_player.html)
* [More JS API reference](http://support.ooyala.com/developers/documentation/concepts/player_v3_dev_customplayer.html)

## FAQ
### How do I get a playlist ID to add to a player?
Query `/v2/playlists` against ooyala's API. You'll probably do that here: https://api.ooyala.com/docs/api_scratchpad

### How do I get a label ID when I want to add a new category to the site and to the autopost?
Query `/v2/labels` against ooyala's API.
