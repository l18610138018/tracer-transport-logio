# tracer-transport-logio #


A [Log.io](https://github.com/NarrativeScience/Log.io) transport for [Tracer](https://github.com/baryon/tracer). Helps bring your _console.log_ to browser in realtime.


## How to use ?


``` javascript
	var logio = new Logio();

	var logger = require('tracer').colorConsole({
	    transport: logio.transporter    
	});

	logger.log("This will be printed to console & sent to log.io");

```

#### License: [Unlicense](http://unlicense.org/)