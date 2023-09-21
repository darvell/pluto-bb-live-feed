# Big Brother Live Feeds Watcher

In Canada or some other hellhole country? Don't want to go buy a VPN to watch BB live feeds? Here's your solution.

Just go here: https://darvell.github.io/pluto-bb-live-feed/

## How it works

Pluto.tv's API allows sending any X-Forwarded-For IP and takes it as the truth. As a result we can feed any IP in US IP space and get all the channels.
Then a proxy is used to strip the CORS requirements on the m3u8 playlists, as well as modify it so sub-playlists are proxied as well.
Eventually this gets us to files directly on the CDN so the proxy doesn't have to do any work.

Net result: Pluto.tv channels (in our case, the big brother ones) in any country.

