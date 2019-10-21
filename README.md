# Rice_Stress
sub : "SUTN9-2" and "S141" 
pro : "Enzyn activity"

----------------------------------
- **zero dependencies** - while the CL utility and test have dependencies, we will never call out to a module for what is supposed to be this lib's core competancy.
- **color profiles** support - other libraries assume you are running x11
- **no prototype manipulation** - No `String.prototype` usage. No `__proto__` usage. No BS.
- handles the ugly [intersection of **multiline text and ansi codes**](docs/Multiline.md) for you.
- runs in the **browser and Node.js** (CommonJS, AMD, globals or webpack)
 
Styles
------
Add ANSI styles to a string and return the result.

| In your code                                    |         In the [Terminal](docs/Terminal.md)                           |
|-------------------------------------------------|---------------------------------------------------|
| `.style(text, style[, close]) > String`          | `ascii-art text -s green "some text"`             |

Styles are: *italic*, **bold**, <span style="text-decoration: underline">underline</span>, <span style="text-decoration: underline overline">|framed|</span>, <span style="text-decoration: underline overline">|encircled|</span>, <span style="text-decoration: overline">overline</span>, <span style="text-decoration: blink">blink</span> and <span style="display:inline-block; background-color:#777777; color: white">&nbsp;inverse&nbsp;</span>. And available colors are:

| **Color Table**  | `color`       | bright_`color`  | `color`_bg| bright_`color`_bg|
| -----------------|---------------|-----------------|-----------|------------------|
| black   |![color](Images/c/black.png)|![color](Images/c/light_black.png)|![color](Images/c/black.png)|![color](Images/c/light_black.png)|
| red     |![color](Images/c/red.png)|![color](Images/c/light_red.png)|![color](Images/c/red.png)|![color](Images/c/light_red.png)|
| green   |![color](Images/c/green.png)|![color](Images/c/light_green.png)| ![color](Images/c/green.png)|![color](Images/c/light_green.png)|
| yellow  |![color](Images/c/yellow.png)|![color](Images/c/light_yellow.png)|![color](Images/c/yellow.png)|![color](Images/c/light_yellow.png)|
| blue    |![color](Images/c/blue.png)|![color](Images/c/light_blue.png)|![color](Images/c/blue.png) |![color](Images/c/light_blue.png)|
| cyan    |![color](Images/c/cyan.png)|![color](Images/c/light_cyan.png)|![color](Images/c/cyan.png) |![color](Images/c/light_cyan.png)|
| magenta |![color](Images/c/magenta.png)|![color](Images/c/light_magenta.png)|![color](Images/c/magenta.png)|![color](Images/c/light_magenta.png)|
| white   |![color](Images/c/gray.png)|![color](Images/c/light_gray.png)|![color](Images/c/gray.png)|![color](Images/c/light_gray.png)|


Compositing
-----------



Promises
--------

Instead of providing a callback, you can also get a promise instead ( `.toPromise()`).

| In your code                                |
|---------------------------------------------|
| `.font(text, font[, style]).toPromise()`    |



Compatibility
-------------


Roadmap
-------

####Goals
- Better Docs
- Color handling/256 color support
- value reversal (light vs dark)

####Non Goals

- realtime: videos, curses, etc.:
- logging integration


Testing [LAB_1/2]
-------
	
Testing [LAB_2/2]
------- 
