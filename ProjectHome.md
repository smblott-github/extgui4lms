# An Alternative Web Interface for the Logitech Media Server #

![http://extgui4lms.googlecode.com/files/screen.png](http://extgui4lms.googlecode.com/files/screen.png)

### Features ###
  * A desktop-like, responsive and intuitive user interface build with modern web technologies
  * Advanced playlist management
  * Custom search function
  * Statistics with pretty graphs
  * Plus
    * Favorites
    * Internet radio
    * Limited access to plugins
    * Lyrics
    * Album & artist information (via [Discogs](http://www.discogs.com))
    * Artist "social" information (news, blogs, ...) (via the [Music & Artist Information plugin](http://forums.slimdevices.com/showthread.php?99537-Announce-Music-amp-Artist-Information-plugin))
    * ...

![http://extgui4lms.googlecode.com/files/screen2.png](http://extgui4lms.googlecode.com/files/screen2.png)

### Scope ###
This is not, and is not meant to be, a complete replacement for the standard web interface. There is no access to settings and some other advanced functionality, and only fairly limited support for using the GUI of plugins.
The main focus is to show as much real-time information as possible at a glance, to enable quick and easy navigation through the music library, and to make managing the current playlist easier.

### Status ###
It's mostly feature-complete (compared to the initial scope, which has, however, expanded quite a bit since the first release - mostly due to feedback from the Squeezebox Forum), and fairly stable on my setup. I'd still consider it beta quality, though - I'm quite sure there are a number of bugs left.

### Performance ###
The app places a higher load on the server than the standard web interface, since it fetches a lot more information more frequently. It also needs more resources on the client side, due to the completely Javascript-based GUI. That being said, it seems to be fast enough even on fairly low-powered hardware (I tested it on an AMD E-450 powered netbook and it was ok). If your server is slow and your collection is large, you might run into performance issues, though.

### Prerequisites ###
  * A modern web browser
    * Works well on Google Chrome/Chromium and Internet Explorer 9. I'd recommend Chrome/Chromium, though, since it seems to have better Javascript performance.
    * Reported to work on Opera, Safari and IE10
    * Mostly works on Firefox >= 19 (reported to completely work in Firefox Aurora 21, though)
  * If you have a large music collection, your LMS server needs to provide adequate performance

### Installation ###
extGUI4LMS can be installed using Logitech Media Server's Extension Downloader. You should find it in the LMS web interface (Settings/Plugins/Other 3rd party plugins).
If not, add http://extgui4lms.googlecode.com/svn/trunk/repository/repo.xml to the list of Additional Repositories in the Extension downloader plugin settings  (located in Settings/Plugins in the standard web interface) and activate the plugin.
You'll find an entry in the Extras menu, which is just a link (yourlmsserver/plugins/LMSnewGUI/html/app.html), so you could bookmark it - it doesn't have to be launched from the regular web interface.

### Usage Instructions ###
See the built-in help (click on the ? icon at the top of the application)

### Reporting Issues ###
Currently, the best way is to post in the discussion thread in the [LMS Forum](http://forums.slimdevices.com/showthread.php?98186-Announce-Alternative-Web-Interface-(beta))