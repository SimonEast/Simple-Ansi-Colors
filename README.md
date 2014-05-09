Simple Ansi Colors in PHP
==================

Simple PHP class for converting basic HTML-like color tags into ANSI escape codes for use in console apps and scripts.  Auto-detection for Windows/Ansicon users included.

Version 1.0.0

Requires PHP 5.3 or above.

# How to use

1. Include the class in your script: `require('simple-ansi-colors.php');`
2. Output some text: `echo Ansi::tagsToColors('<green>Hello <yellow>World!');`

# Supported tags

 <black>
 <red>
 <green>
 <yellow>
 <blue>
 <magenta>
 <cyan>
 <white>
 <gray>
 <darkRed>
 <darkGreen>
 <darkYellow>
 <darkBlue>
 <darkMagenta>
 <darkCyan>
 <darkWhite>
 <darkGray>
 <bgBlack>
 <bgRed>
 <bgGreen>
 <bgYellow>
 <bgBlue>
 <bgMagenta>
 <bgCyan>
 <bgWhite>
 <bold>
 <italics>
 <reset>

Run `php demo.php` to view a sample of all the options available.  In consoles with ANSI color support, you'll see the following...

 ![Color screenshot](http://img845.imageshack.us/img845/1201/5gge.png)

In the Windows command prompt (without AnsiCon), color tags will simply be stripped out.

 ![Non-color screenshot](http://img834.imageshack.us/img834/5667/3p1t.png)

Windows users can [download AnsiCon](https://github.com/adoxa/ansicon/releases) and install it by running `ansicon -i` from a command prompt or "Run" window.  This will allow them to view colors.
