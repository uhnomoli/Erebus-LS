# Erebus LS

A [LiteStep][1] theme roughly based on my [TextMate theme][2] of the same name.


### Thanks

First, I'd like to quickly give thanks to the people that helped me make this theme what it is.

+ __Greywool__ and __alurcard2__ over in __#litestep[___freenode___]__ were a big help. They helped me out a lot when it came to the odd one off issues I encountered. Thanks to both of you guys.
+ __Everyone__ in __[#pixelfuckers][3][___freenode___]__ for putting up with all my pestering and giving me their opinions on it's progress. You could hop in there at any given time and chances are each person in there has helped me out in some form at some point. Thanks to all of you guys as well.


### Notes

All modules should download just fine if you don't already have them with the __exception__ of __jDesk 0.75__. You can find it in [this][4] _([direct link][5])_ news post as well as in `/Extras`. Just extract the dll to `LiteStep/modules`. If for any reason, any other module can't be downloaded, you should be able to find it either [here][6], [here][7], or [here][8].

This theme __requires__ the font [Semplice Regular][9] _([download][10])_ which can also be found in `/Extras`.


### Configuration

The widgets are the only things that really require configuration.

#### Album Art

The album art widget will search the folder the music is being played from first for cover art after which it will check the ID3 tags. You should configure `erbAlbumArtCoverName` to whatever your library uses. If you have multiple naming schemes you can configure that like so:

    erbAlbumArtCoverName "cover.jpg" "folder.jpg" "albumart.png"

If more than one of those files are found for the currently playing track, whichever is listed first will be used. _(For example, if both cover.jpg and albumart.png were found for the current track, with the above setting, cover.jpg would be used.)_

__NOTE:__ If you are not using Winamp you need to find if your player has a plugin that emulates Winamp messages and install it. For example, if you are using foobar2000, you need to install [foo_vis_shpeck][11].

__NOTE:__ The album art widget will only be displayed if album art is found for the currently playing track. It will automatically fade in and out while listening to music depending on whether or not album art is found.

#### Net Stats

The net stats widget doesn't really require any configuration and will work with the default settings. However, depending on your connection, you may wish to change `erbNetInScale` and `erbNetOutScale` in `config/themeVars.rc`. These two settings control each graph's maximum _(in kB/s)_. For example, if you set `erbNetInScale` to 500, and were downloading a file at 250 kB/s, your download speed would be plotted in the middle of the graph.

#### Weather

To configure the weather widget you need to find your [WOEID][12]. To do this goto [http://weather.yahoo.com/][13]. Enter your area code or city in the appropriate box and hit enter. You will be taken to a page with a URL in this format: `http://weather.yahoo.com/<country>/<state>/<city>-<WOEID>/` Simply grab the WOEID from the URL and set `erbWeatherWOEID` in `config/themeVars.rc` to it.


### Theme Popup

The following settings are configurable from the theme popup _(middle click the desktop to access it)_. The only option that triggers / requires a recycle to take effect is changing shadows.

_Bold signifies the default setting._

+ __Global__
    + Shadows _(__on__/off)_
+ __Popup__
    + Font Color _(__orange__/red)_
    + Separator Style _(__space__/line/akka)_
+ __Sys Tray__
    + Icon Desaturation _(__on__/off)_
+ __Widgets__
    + Stats
        + Start Hidden _(on/__off__)_
    + Album Art
        + ___Enable___
        + _Disable_


### Various Functionality

+ __Desktop__
    + Middle click, brings up the theme popup.
+ __Start Button__
    + Right click, minimizes all windows.
+ __Taskbar__
    + Middle click, closes the task clicked.
+ __Clock__
    + Left click, toggles the sys tray.
+ __Clock Icon__
    + Left click, toggles the stats widgets.
    + Right click, toggles the album art widget.
+ __Weather Widget__
    + Left click, opens your browser to your local weather.


### Credits

+ __Font__
    + [Semplice Regular][9] by Michael Schmidt
+ __Start Menu Icons__
    + [Tango][14] by Tango Desktop Project
    + [Boolean 1.1][15] _(recycle bin)_ by PraX-08
+ __Weather Icons__
    + [Plain Weather Icons][16] by MerlinTheRed


### Preview

[![Preview][100]][17]


[1]: http://www.litestep.net/
[2]: http://github.com/uhnomoli/Erebus.tmTheme
[3]: http://pixelfuckers.org/
[4]: http://www.ls-universe.ls-themes.org/comment.php?comment.news.550
[5]: http://dl.dropbox.com/u/51925/LiteStep/jDesk-0.75.zip
[6]: http://xdocs.ls-universe.ls-themes.org/doku.php?id=litestep:modules:modules
[7]: http://www.ls-themes.org/modules/
[8]: http://www.modules.shellfront.org/
[9]: http://www.style-force.net/work/type/pixelfonts
[10]: http://www.style-force.net/pixelfonts/semp_reg.zip
[11]: http://www.foobar2000.org/components/view/foo_vis_shpeck
[12]: http://developer.yahoo.com/geo/geoplanet/guide/concepts.html
[13]: http://weather.yahoo.com/
[14]: http://tango.freedesktop.org/
[15]: http://prax-08.deviantart.com/art/Boolean-1-1-166457851
[16]: http://merlinthered.deviantart.com/art/plain-weather-icons-157162192
[17]: http://github.com/uhnomoli/Erebus-LS/raw/master/Extras/Screens/full.jpg

[100]: https://github.com/uhnomoli/Erebus-LS/raw/master/Extras/Screens/thumb.jpg

