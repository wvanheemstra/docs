Title: README  
Author: Willem van Heemstra  
Affiliation: van Heemstra Systems  
Copyright: All rights reserved - van Heemstra Systems

#docs/skin/README.md
The skin documentation.
![Image](../skin/images/system_overview_skin.png?raw=true)  System Overview - Skin

##About skin
Skin is the **layout** layer.

[Dependencies](#Dependencies)  
[Installation](#Installation)  
[Testing](#Testing)  
[Server](#Server)  
[License](#License)  

##<a id="Dependencies"></a>Dependencies
For web clients (mobile, phone and desktop), the Sencha Touch and ExtJS libraries are used. See [Sencha](http://www.sencha.com/)

To manage the individual views and view models, in addition, GluJS is used. See [GluJS](http://conarrative.github.io/glujs-guide/)

##<a id="Installation"></a>Installation
Installation is by making the directory 'public' accessible from your web root.

Run nmp install from within the public/app/ folder to install the node modules listed in package.json.

##<a id="Testing"></a>Testing
Following the path to the 'public' web folder should show you the index.html page.

By default, Jasmine is used for testing specs. See [Jasmine](http://pivotal.github.io/jasmine/)

Testing of the spec for web clients can be done by running the SpecRunner.html inside path-to/public/app/spec/ 

Testing on the server (using NodeJS) uses the same spec.

See Manuel Kiessling's blog post, where he explains how to test for either client or server side javascript specs at [True Universal Javascript Modules with Write Once Run Anywhere Jasmine Specs](http://manuel.kiessling.net/2012/03/30/true-universal-javascript-modules-with-write-once-run-anywhere-jasmine-specs/)

Specs are written in CoffeeScript and parsed to JavaScript.

##<a id="Server"></a>Server
You can use your own preferred web server.

##<a id="License"></a>Licence
(The MIT License)

Copyright (C) 2013 Willem van Heemstra willem@vanheemstrasystems.com

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the 'Software'), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.