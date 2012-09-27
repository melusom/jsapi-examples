# About

This web-app is an example usage of the new Rdio JavaScript API. You can see it in action at http://music-triage.appspot.com/

I like to queue up a bunch of new music and listen to it throughout the day. Every day or two I go back through my history and add the albums I liked to my collection. This web app is tailored to that history triage. Albums you've listened to but haven't triaged show up in the middle. Hit the heart on an album to add that album to your collection; hit the X to discard it.

Note that the "dustbin" status of an album is stored only in your browser's local storage. Perhaps in the future we'll add a server-side component for more robust storage.

# Todo: high

* Handle individual tracks properly: either ignore them entirely or do the full album
* Handle play lists as well as albums, or ignore them for now
* Show track count (when album is shown big)
* Don't add the same album to the triage list twice
* Layout animation doesn't seem to be working (heart/X)
* Save dustbin to server

# Todo: normal

* If an album is playing when you hit heart/x, start the next album playing
* Each click on sample button should take you to 1/3rd through the next track (on playingTrack change, seek to its duration / 3)
* Album and artist name
* Indicate that there's nothing left to triage when you're all done
* Key combos
* The first time you hit play there's a bit of a lag before the button highlights
* Shadows behind buttons

# Todo: low

* Spinner for buffering
* Periodically check for newly played albums
* Only load as much collection as needed (remember where you left off)
* Third option: add back to the queue for another listen
* Use normal Rdio album controls, but add some of our own
* Triage for new releases (heart goes into queue instead of collection)
* Sort high if other albums from same artist in collection; low if not and others in dustbin