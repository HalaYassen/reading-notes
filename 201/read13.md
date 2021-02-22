* Cookies 
cookies were invented early in the web’s history, and indeed they can be used for persistent local storage of small amounts of data.
But they have three potentially dealbreaking downsides:

1. Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over
2. Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)
3. Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful.

**but really we need** (a lot of storage space, on the client that persists beyond a page refresh and isn’t transmitted to the server).

* HISTORY OF LOCAL STORAGE HACKS BEFORE HTML5:

* there was only Internet Explorer in the beginning, Microsoft invented a great many things and included them in their browser-to-end-all-browser-wars, Internet Explorer. One of these things was called `DHTML` Behaviors, and one of these behaviors was called userData.

*userData* allows web pages to store up to 64 KB of data per domain.

* **In 2002**, Adobe introduced a feature in Flash 6 that gained the unfortunate and misleading name of “Flash cookies.” Within the Flash environment, the feature is properly known as Local Shared Objects. Briefly, it allows Flash objects to store up to 100 KB of data per domain. Brad Neuberg developed an early prototype of a Flash-to-JavaScript bridge called AMASS (AJAX Massive Storage System), but it was limited by some of Flash’s design quirks. By 2006, with the advent of ExternalInterface in Flash 8, accessing LSOs from JavaScript became an order of magnitude easier and faster. Brad rewrote AMASS and integrated it into the popular Dojo Toolkit under the moniker dojox.storage. Flash gives each domain 100 KB of storage for free.

* **In 2007**, Google launched Gears, an open source browser plugin aimed at providing additional capabilities in browsers. (We’ve previously discussed Gears in the context of providing a geolocation API in Internet Explorer.) Gears provides an API to an embedded SQL database based on SQLite. After obtaining permission from the user once, Gears can store unlimited amounts of data per domain in SQL database tables.

### USING HTML5 STORAGE

HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including (strings, Booleans, integers, or floats(), the data is actually stored as a string. 

* If you are storing and retrieving anything other than strings, you will need to use functions like `parseInt()` or `parseFloat()` to coerce your retrieved data into the expected JavaScript datatype.

## LIMITATIONS IN CURRENT BROWSERS
“5 megabytes” is how much storage space each origin gets by default. This is surprisingly consistent across browsers, although it is phrased as no more than a suggestion in the HTML5 Storage specification. One thing to keep in mind is that you’re storing strings, not data in its original format. If you’re storing a lot of integers or floats, the difference in representation can really add up. Each digit in that float is being stored as a character, not in the usual representation of a floating point number.

**`QUOTA_EXCEEDED_ERR`** is the exception that will get thrown if you exceed your storage quota of 5 megabytes, no browser supports any mechanism for web developers to request more storage space. Some browsers like Opera allow the user to control each site’s storage quota, but it is purely a user-initiated action, not something that you as a web developer can build into your web application.

