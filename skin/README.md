Title: README  
Author: Willem van Heemstra  
Affiliation: van Heemstra Systems  
Copyright: All rights reserved - van Heemstra Systems

#docs/skin/README.md
====
The skin documentation.
![Image](../skin/images/system_overview_skin.png?raw=true)  System Overview - Skin

##About skin
Skin is the **layout** layer.

[Installation][]  
[Testing][]  
[Server][]  

##Installation [Installation]##
Installation makes use of Node Package Manager [npm], see [http://npmjs.org](http://npmjs.org).

To install all dependencies of skin with npm, from the skin directory that contains package.json, type:

	```
	#path-to-skin/npm install
	```

##Testing [Testing]
Testing makes use of Mocha, see [http://visionmedia.github.io/mocha](http://visionmedia.github.io/mocha).

##Server [Server] ##
Hem Server is used, see [http://npmjs.org/package/hem](http://npmjs.org/package/hem).

Starting the server (e.g. port 80, ip 127.0.0.1):

	```
	#path-to-skin/hem server -p 80 -host 127.0.0.1
	```

##Licence
(The MIT License)

Copyright (C) 2013 Willem van Heemstra willem@vanheemstrasystems.com

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the 'Software'), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.