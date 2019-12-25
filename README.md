# habpanel-widget-SpotifyControlWithArt
thanks to these nice widgets

* [Squeezebox controller widget](https://community.openhab.org/t/squeezebox-controller-widget/47260)
* [Habpanel Sonos Widgets](https://community.openhab.org/t/habpanel-sonos-widgets/70987)

which I combined - or took as template - I came up with this widget for spotify.

I tried to be as close as possible to the Windows App in the layout of the controls.

Some changes had to be done *(or I didn*t know how to do them)* though
* volume control is below player control 
  * as I didn't want to make to controls too small 
  * or too wide
* The current [Spotify Binding](https://www.openhab.org/addons/bindings/spotify/) unfortunately does not provide a Mute property.
  * So I added a volume control next to the volume slider
  * if someone knows how to 
    * save the last volume on press of the mute button, 
    * restore on next press
please let me know
* I used official spotify icons whereever I could find them but some icons I could not find in the spotify developer pages
  * mute
  * queue
  * available devices

features to come (if I find a nice way how to put it in)
* support for playlists
* support for favorites
* mute control (see above)
* hoverover for the controls - to make them green :-) 

**Screenshot**
* plausing
![SpotifyControlWithArt|399x500](upload://anOIfBuTzPHrOEbfMig1884dzH.jpeg) 
* playing with shuffle active
![SpotifyControlWithArt_shuffle|397x500](upload://4NCThOEoYRJYLjq0Xe6TQ31AXEl.jpeg) 

**How to install**
* enable the [Spotify Binding](https://www.openhab.org/addons/bindings/spotify/)
* make sure it works
* enable to following items in the **Spotify Player Bridge**
  * Volume
  * Active Device Shuffle
  * Media Control
  * Repeat Mode
  * Media Title
  * Track Progress (ms)
  * Track Duration (ms)
  * Album Image
  * Media Artist
* add the widget to your library
  * **[habpanel-widget-SpotifyControlWithArt](https://github.com/Rosi2143/habpanel-widget-SpotifyControlWithArt)**
* add the icons to the html directory of your openHAB installtion.
  * [Linux](https://www.openhab.org/docs/installation/linux.html#file-locations)
    * /etc/openhab2
  * [Windows](https://www.openhab.org/docs/installation/windows.html#file-locations)
    * C:\openHAB2\conf 
  * others see [here](https://www.openhab.org/docs/installation/)

I hope you like this widget.
