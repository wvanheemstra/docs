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

To manage the individual views, models, stores, controllers, mediators and services , in addition, FlowMVC is used. See [FlowMVC](https://github.com/WebAppSolutionInc/flow-mvc)

To serve the files, ExpressJS is used. See [ExpressJS] (http://expressjs.com/)

##<a id="Installation"></a>Installation
Installation is by making the directory 'public' accessible from your web root.

Run 'nmp install' from within the root to install the node modules listed in package.json.

Place the following packages in the public folder:

/public/resources/js/ext/ [PUT THE SENCHA EXT PACKAGE HERE]  
/public/resources/js/touch/ [PUT THE SENCHA TOUCH PACKAGE HERE]  

Copy, rename and customise the following sample files:

/server/server-starter.bat.sample  TO /server/server-starter.bat  
/server/server-starter.sh.sample  TO /server/server-starter.sh  
/public/index.ejs.sample  TO /public/index.ejs  
/public/index-debug.ejs.sample  TO /public/index-debug.ejs  
/public/index-touch.ejs.sample  TO /public/index-touch.ejs  
/public/app/config/global/Config.js.sample  TO /public/app/config/global/Config.js  
/public/resources/icons_loading_startup.ai.sample  TO /public/resources/icons_loading_startup.ai

Copy, rename and customise the following image files to fit your application:

/public/resources/icons/ [IMAGES WITH .sample]  TO /public/resources/icons/ [IMAGES WITHOUT .sample]  
/public/resources/loading/ [IMAGES WITH .sample]   TO  /public/resources/loading/ [IMAGES WITHOUT .sample]  
/public/resources/startup/ [IMAGES WITH .sample]   TO  /public/resources/startup/ [IMAGES WITHOUT .sample]  
/public/favicon.png.sample  TO  /public/favicon.png  
/public/favicon.ico.sample TO /public/favicon.ico   

NOTE: Use this site: [ConvertIcon](http://converticon.com/) to convert your image file to an *.ico file. Recommended size is 16px * 16px.

NOTE: An Adobe Illustrator file is supplied (copied and renamed as per above instructions) for easy re-designing of your image files. See:

/public/resources/icons_loading_startup.ai  

##<a id="Testing"></a>Testing
Following the path to the 'public' web folder should show you the index.html page.

By default, Jasmine is used for testing specs. See [Jasmine](http://pivotal.github.io/jasmine/)

Testing of the spec for web clients can be done by running the SpecRunner.html inside path-to/public/app/spec/ 

Testing on the server (using NodeJS) uses the same spec.

See Manuel Kiessling's blog post, where he explains how to test for either client or server side javascript specs at [True Universal Javascript Modules with Write Once Run Anywhere Jasmine Specs](http://manuel.kiessling.net/2012/03/30/true-universal-javascript-modules-with-write-once-run-anywhere-jasmine-specs/)

Specs are written in CoffeeScript and parsed to JavaScript.

##<a id="Server"></a>Server
To start the web server, run 'node server.js' from within the /server folder. The site will then be accessible on http://\<your host>:\<your port number>

The server will distinguish between client device types (e.g. desktop, mobile, tablet, tv etc), thanks to express-device. See [express-device](https://github.com/rguerreiro/express-device)

For Windows one can run a batch file to start the server:  
/server/server-starter.bat

For Unix one can run a shell file to start the server:  
/server/server-starter.sh

By default, the server.js will run for 'development environment'.  
Overwrite to 'production environment' (e.g. uses caching) as follows:

export NODE_ENV=production  
node server.js

##<a id="License"></a>Licence
(The MIT License)

Copyright (C) 2013 van Heemstra Systems info@vanheemstrasystems.com

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the 'Software'), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.