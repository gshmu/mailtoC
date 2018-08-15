mailtoC
=======
Copy mailto address to clipboard under mac os x

# require
- max OS X: applescript Editor
- RCDefaultApp |or| mail

## build Application
open ./mailtoC by applescript Editor or create new applescript
```apple script
on open location mailtostr
	try
		tell application "Finder" to set the clipboard to text 8 thru end of mailtostr
	end try
end open location
```
Using applescript `File` --> `Export` Application type. (I'm Export as Application, Script bundle may work too.)

## change default
suggest using [RCDefaultApp](http://www.rubicode.com/Software/Bundles.html#RCDefaultApp)
change default mail to mailtoC exported Application.

# thanks
http://kwiniec.altervista.org/ff3fixes_files/mailto.html

