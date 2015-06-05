# tracer-transport-logio #


A [Log.io](https://github.com/NarrativeScience/Log.io) transport for [Tracer](https://github.com/baryon/tracer). Helps bring your _console.log_ to browser in realtime.


## How to use ?


``` javascript
	var logio = new Logio();

	var logger = require('tracer').colorConsole({
	    transport: logio.transporter    
	});

	logger.json = function() {
	    for (var key in arguments) {
	        this.info(JSON.stringify(arguments[key], null, 2));
	    }
	};

	module.exports = logger;

```

#### License: [Unlicense](http://unlicense.org/)