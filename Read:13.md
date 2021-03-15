## A BRIEF HISTORY OF LOCAL STORAGE HACKS BEFORE HTML5

In the beginning, there was only Internet Explorer. Or at least, that’s what Microsoft wanted the world to think. To that end, as part of the First Great Browser Wars, Microsoft invented a great many things and included them in their browser-to-end-all-browser-wars, Internet Explorer. One of these things was called DHTML Behaviors, and one of these behaviors was called userData.

userData allows web pages to store up to 64 KB of data per domain, in a hierarchical XML-based structure. (Trusted domains, such as intranet sites, can store 10 times that amount. And hey, 640 KB ought to be enough for anybody.) IE does not present any form of permissions dialog, and there is no allowance for increasing the amount of storage available.

In 2002, Adobe introduced a feature in Flash 6 that gained the unfortunate and misleading name of “Flash cookies.” Within the Flash environment, the feature is properly known as Local Shared Objects. Briefly, it allows Flash objects to store up to 100 KB of data per domain. Brad Neuberg developed an early prototype of a Flash-to-JavaScript bridge called AMASS (AJAX Massive Storage System), but it was limited by some of Flash’s design quirks. By 2006, with the advent of ExternalInterface in Flash 8, accessing LSOs from JavaScript became an order of magnitude easier and faster. Brad rewrote AMASS and integrated it into the popular Dojo Toolkit under the moniker dojox.storage. Flash gives each domain 100 KB of storage “for free.” Beyond that, it prompts the user for each order of magnitude increase in data storage (1 Mb, 10 Mb, and so on).

In 2007, Google launched Gears, an open source browser plugin aimed at providing additional capabilities in browsers. (We’ve previously discussed Gears in the context of providing a geolocation API in Internet Explorer.) Gears provides an API to an embedded SQL database based on SQLite. After obtaining permission from the user once, Gears can store unlimited amounts of data per domain in SQL database tables.

In the meantime, Brad Neuberg and others continued to hack away on dojox.storage to provide a unified interface to all these different plugins and APIs. By 2009, dojox.storage could auto-detect (and provide a unified interface on top of) Adobe Flash, Gears, Adobe AIR, and an early prototype of HTML5 storage that was only implemented in older versions of Firefox.

As you survey these solutions, a pattern emerges: all of them are either specific to a single browser, or reliant on a third-party plugin. Despite heroic efforts to paper over the differences (in dojox.storage), they all expose radically different interfaces, have different storage limitations, and present different user experiences. So this is the problem that HTML5 set out to solve: to provide a standardized API, implemented natively and consistently in multiple browsers, without having to rely on third-party plugins.

## HTML5 STORAGE

![](https://blog.teamtreehouse.com/wp-content/uploads/2013/01/localstorage-feature.png)

it’s a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you. Unlike cookies, this data is never transmitted to the remote web server (unless you go out of your way to send it manually), Unlike all previous attempts at providing persistent local storage, it is implemented natively in web browsers, so it is available even when third-party browser plugins are not.

## USING HTML5 STORAGE
HTML5 Storage is based on named key/value pairs, You store data based on a named key, then you can retrieve that data with the same key, The named key is a string, The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string, If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype.


## LIMITATIONS IN CURRENT BROWSERS

“5 megabytes” is how much storage space each origin gets by default.

Each digit in that float is being stored as a character, not in the usual representation of a floating point number.

Some browsers (like Opera) allow the user to control each site’s storage quota, but it is purely a user-initiated action, not something that we as a web developer can build into our web application.

In 2007, Google launched Gears, an open source cross-browser plugin which included an embedded database based on SQLite.

Web SQL Database (formerly known as “WebDB”) provides a thin wrapper around a SQL database, allowing us to do things like this from JavaScript:

openDatabase(‘documents’, ‘1.0’, ‘Local document storage’, 510241024, function (db) { db.changeVersion(‘’, ‘1.0’, function (t) { t.executeSql(‘CREATE TABLE docids (id, name)’); }, error); });

There’s Oracle’s SQL, Microsoft’s SQL, MySQL’s SQL, PostgreSQL’s SQL, and SQLite’s SQL. Indeed, each of these products adds new SQL features over time, so even saying “SQLite’s SQL” is not sufficient to pin down exactly what we’re talking about. We need to say “the version of SQL that shipped with SQLite version X.Y.Z.”

The Indexed Database API exposes what’s called an object store. An object store shares many concepts with a SQL database. There are “databases” with “records,” and each record has a set number of “fields.” Each field has a specific datatype, which is defined when the database is created. We can select a subset of records, then enumerate them with a “cursor.” Changes to the object store are handled within “transactions.”

## What do different browsers have to say about IndexedDB?
At time of writing, IndexedDB has only been implemented in a beta version of Firefox 4.

(By contrast, **Mozilla** has stated that they will never implement Web SQL Database.) Google has stated that they are considering IndexedDB support for Chromium and Google Chrome. And even Microsoft has said that IndexedDB “is a great solution for the web.”

So what can you, as a web developer, do with IndexedDB?
At the moment, virtually nothing beyond some technology demos. A year from now? Maybe something. Who knows