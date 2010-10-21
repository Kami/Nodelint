Color.js
========


Color.js is a coloring module for text output to the terminal.



Color.*color*( string )
-----------------------

The color module comes with a predefined set of colors: red, green, blue & yellow  
It also comes with their bold counter parts: boldred, boldgreen, boldblue & boldyellow


Usage
=====

	// Color Module
	var Color = require('Nodelint/lib/nodelint/Color').Color, sys = require('sys');

	// Shortcut to coloring a string red for terminal output
	sys.puts( Color.red( 'This is a red string' ) );
