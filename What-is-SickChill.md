#### What is SickChill?

SickChill is a program that downloads your favorite TV shows, and then processes and stores them in your library.
And that is all fully automated! Just set it up and as soon as there is a new episode released it gets downloaded. SickChill is your ultimate PVR!

#### How does this all work?

When you add a show to SickChill the data (like air-dates, episode name/number) are pulled from an indexer like [TheTVDb](http://thetvdb.com/). At that point, SickChill knows when a new episode is going to air and starts the search on your favorite Torrent and/or NZB site. For this search you can set [quality](Quality-Settings) settings. For example: HDTV or SD quality. SickChill will go over all the results to find the [quality](Quality-Settings) YOU want and when found snatches the torrent/nzb and sends it to your download client. (sabnzb, utorrent, transmission etc.) At this point, SickChill starts monitoring your client's download folder to see if the file is finished downloading. When this is the case SickChill starts the post-processing. Here you can tell SickChill to move the file to your shows folder, or also rename it, or send notifications to Plex/Kodi or to your smartphone. The list is long for what you can do with post-processing, simply set the actions you prefer.
And this whole process is completely automated. So once you set it up no user intervention is required.
This makes SickChill ideal for NAS devices. But can run on almost every other device.

#### Features

SickChill contains a ton of cool features. Some of those are :

- Automatic torrent/nzb searching, downloading, and processing at the qualities you want
- Automatic subtitle downloads for your shows.
- Supports Anime and Sports shows
- Largest list of build-in torrent and nzb providers, both public and private
- Possibility to add (almost) every NZB/Torrent provider with the custom provider option
- Sends notifications to your media server/software and/or mobile/social devices
- Can notify Kodi, XBMC, Growl, Trakt, Twitter, and many more when new episodes are available
- Updates Kodi library, poster/banner/fanart downloads, and NFO/TBN generation
- Configurable automatic episode renaming, sorting, and other post-processing
- Easily see what episodes you're missing, are airing soon, and more
- Searches TheTVDB.com and AniDB.net for shows, seasons, episodes, and metadata
- Episode status management allows for mass failing seasons/episodes to force retrying
- DVD Order numbering for returning the results in DVD order instead of Air-By-Date order
- Allows you to choose which indexer to have SickChill search its show info from when importing
- Automatic XEM Scene Numbering/Naming for seasons/episodes
- Available for any platform, uses a simple HTTP interface
- Specials and multi-episode torrent/nzb support
- Improved failed download handling
- DupeKey/DupeScore for NZBGet 12+
- Real SSL certificate validation

#### Screenshots

_(as of December 2014)_<br/> -[Desktop (Full-HD)](http://imgur.com/a/4fpBk)<br> -[Mobile](http://imgur.com/a/WPyG6)

#### Dependencies

To run SickChill we recommend [Python 3.8 or higher](https://www.python.org/downloads/), Python 3.7 as minimum.  
The latest modules of [Pip](https://pypi.org/project/pip),
[Poetry](https://pypi.org/project/poetry), [PyOpenSSL](https://pypi.python.org/pypi/pyOpenSSL), and [cryptography](https://pypi.python.org/pypi/cryptography).  
SickChill will load many other packages from [Pypi](https://pypi.org/) too.

#### Support

In case the [Wiki](https://github.com/SickChill/SickChill/wiki) doesn't have the answer to your question, you could check us out on [Discord](https://discord.gg/U8WPBdf).

#### Bugs/Issues

In case you have found a bug and verified that it indeed is a bug, then please report it to our [Discord help channel](https://discord.com/channels/502612977271439372/1048317980343283733) so that the Developers can investigate.

---

Disclaimer: SickChill should only be used with shows that you already own or are in the public domain.
