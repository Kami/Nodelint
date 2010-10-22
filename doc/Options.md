Options.js
==========

Options.js contains the options object of default settings for Nodelint and JSLINT. There are three sections.



nodelint
--------

This object contains all the default settings for Nodelint the project.

	// Nodelint options
	{
	  logfile: Path to a logfile to store the results. Defaults to null.
	  jslint: Path to custom JSLINT file. Defaults to null.
	}


jslint
------

JSLINT specific options that just get passed to the JSLINT parser.



shortcuts
----------

Object containing shortcut references for Nodelint options. Each shortcut must use the following format

	"character": {
		"long": longhand reference
		"expect": Boolean, true if option expects an argument to follow, false to just use the default
		"default": Default value for when the shortcut is used without an expectation
	}

An example would be

	// Shortcut for logfile, expecting next argument to be path to logfile
	'l': {
		'long': 'logfile',
		'expect': true,
		'default': null
	}



Usage
=====

	// Not much too it, just returns the options object
	var Options = require('Nodelint').Options;
