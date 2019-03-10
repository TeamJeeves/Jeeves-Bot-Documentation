# Play Command

The play command is a Discord audio player capable of playing audio from a variety of sources.  
The primary source is YouTube, however support is available for other popular streaming services like SoundCloud.  

**Important Note:** Any service that would otherwise require you to login to listen to their music (Spotify/Pandora) can not be used by Jeeves.

### Finding Audio
* **Search YouTube** `!play Hollywood Firework` - Search YouTube for a track matching `Hollywood Firework`
* **YouTube links** `!play https://www.youtube.com/watch?v=KSFVuMT77eg` - Plays the track linked
* **YouTube playlist** `!play https://www.youtube.com/playlist?list=PLA1D6023F6FF2684B` - Import the whole playlist into your queue
***
### Details
**Aliases:** `play`  
**Available in DM:** No  
**Can Restrict to a channel:** Yes    

***

### Examples

* `!play Timber - Pitbull`
> Searches for Timber - Pitbull and puts it in the queue.
* `!play Timber - Putbull --time 1:34`
> Searches for Timber - Pitbull and puts it in the queue, but starts at 1:34
* `!play Timber - Putbull --volume 50`
> Searches for Timber - Pitbull and plays it on 50% volume
* `!play Timber - Pitbull --volume 50 --time 1:34 --playnow`
> This will play the Timber - Pitbull song at 50% volume, at 1:34 and will put it in the front of the playlist


### FAQ
#### (Q) Is it possible to get Spotify to work with Jeeves?
>No, at the moment the following sources are supported:
* YouTube playlists
* YouTube videos
* YouTube livestreams
* SoundCloud
* Random (Try it! If it works, great! If not ... ¯\\\_(ツ)_/¯)
***
