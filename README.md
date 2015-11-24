Simple ANSI Colors in PHP
==================

Simple PHP class for converting basic HTML-like color tags into ANSI escape codes for use in console apps and scripts.

Can be disabled through a single variable so that no colors are output (such as if the output needs to be piped to another app or script).

Auto-detection for Windows/ANSICON users included. Colors are disabled by default on Windows unless ANSICON is detected.

Version 1.0.1
<br>MIT Licence
<br>Requires PHP 5.3 or above.

# How to use

1. Include the class in your script: `require('simple-ansi-colors.php');`
2. Output some text: `echo Ansi::tagsToColors('<green>Hello <yellow>World!');`

Note that unlike HTML, there are no closing tags. Simply use `<reset>` to return the color to the default. For example...

```
<green>This text will be green. <reset>This text will return to the default color.
```

# Supported tags

```
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
```

Run `php demo.php` to view a sample of all the options available. In consoles with ANSI color support, you'll see the following...

![Color screenshot](https://img845.imageshack.us/img845/1201/5gge.png)

In the Windows command prompt (without ANSICON), color tags will simply be stripped out.

![Non-color screenshot](https://img834.imageshack.us/img834/5667/3p1t.png)

Windows users can [download ANSICON](https://github.com/adoxa/ansicon/releases) and install it by running `ansicon -i` from a command prompt or "Run" window. This will allow them to view colors.
