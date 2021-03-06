# ╰(*°▽°*)╯ Giffing Wall Sentimental ╰(*°▽°*)╯

Display a wall of GIFs driven by a simple Twitch live chat sentiment analysis and the Gif search API of your choice (Tenor and Giphy currently available).

## Getting started
* Download or clone the repo. 
* In `/dist/` rename `config.default.js` to `config.js` and follow the instructions there to finish setting things up. 
* If you only want to display a single GIF at a time, set the `gifs.displayCount` config value to `1` - GIFs will be centred in the output window and sized to fit the available space, while maintaining their aspect-ratio.
* Open dist/index.html in a browser or assign as a browser-source in OBS etc.


For faster config changes (or, for example, to run multiple different configs in different windows) any of the config key:value pairs can be overridden via the querystring, like...
* index.html?channel=myFavouriteStreamer&gifs.gifAPIProvider=tenor&gifs.minimumDisplayTime=5

## Examples

A test [Twitch Stream](https://www.twitch.tv/videos/856384544) with a 5-column gif wall reacting to an active channel's chat.

#### Single item with a portrait image fitting to a landscape window area (default mode)
![single-item-example](https://mikedotalmond.co.uk/lab/giffingsentimental/singlegif.png)

#### 5-column wall
![example](https://mikedotalmond.co.uk/lab/giffingsentimental/gifwall.jpg)


## Build
* `npm install`
* `npm run build` or `npm run build-prod`

#### Uses:
* [tmi](https://www.npmjs.com/package/tmi)
* [compromise](https://www.npmjs.com/package/compromise)
* [afinn-165](https://www.npmjs.com/package/afinn-165)
* [masonry-layout](https://www.npmjs.com/package/masonry-layout)
* [timers-browserify](https://www.npmjs.com/package/timers-browserify)
* [webpack](https://www.npmjs.com/package/webpack)
* [webpack-cli](https://www.npmjs.com/package/webpack-cli)
