ChinStrap
=========
ChinStrap is some basic boilerplate code, generated originally by [Yeoman](http://yeoman.io), and massaged by yours truly, taking a nod from [Bootswatch](https://github.com/thomaspark/bootswatch/) to use Bootstrap LESS instead of SCSS and the themeing conventions of bootswatch.

Requirements
------------
ChinStrap requires [Node.js](http://nodejs.org/), and npm to be installed. ChinStrap also requires [Grunt](http://gruntjs.com/) and [Bower](http://twitter.github.com/bower). Yeoman is not required, however the project was generated with `v1.0beta`, so go [check them out](http://yeoman.io).

Install Guide
-------------
1. Install Node & npm.
2. Install Grunt and Bower (may require sudo):
    
        npm install -g grunt-cli bower

3. Clone this repository to create your app (replace myapp with the foldername of your choice):
        
        git clone https://github.com/bdunn313/ChinStrap.git myapp

4. move into your app and install dependencies (see `package.json` and `component.json`):
        
        cd myapp && grunt install && bower install

5. Start the local server:
        
        grunt server


Usage
-----
ChinStrap allows you to create custom theme files in a manner similar to the method used by [Bootswatch](https://github.com/thomaspark/bootswatch/), but without the need for a makefile. Instead, grunt spools up a node webserver for you to use in development, and watches / compiles as you edit less files, without having to edit bootstrap's core less files directly.

Less files are in the `styles` folder. `styles/theme` has your two theme files, `themefile.less` and `vars.less`.
- `themefile.less` is where you place your bootstrap overrides that cannot be achieved simply by changing variables.
- `vars.less` is a mirror of the variables in the main bootstrap `variables.less`. Change these values to modify most of the look and feel of bootstrap.

`styles/main.less` is where you place all of your app-specific styles. The idea is you could potentially save and reuse the files in styles/theme, so anything application/website/project specific should be kept in main.less (or additional less files).

If you want to create another theme, simply duplicate the `styles/theme` directory, and change the corresponding imports in main.less.

Author
------
[Brad Dunn](http://github.com/bdunn313)

http://braddunn.com/

Thanks
------
[Mark Otto](http://github.com/markdotto) and [Jacob Thornton](http://github.com/fat) for [Bootstrap](https://github.com/twitter/bootstrap).

The [Yeoman](http://yeoman.io), [Grunt](http://gruntjs.com/), and [Bower](http://twitter.github.com/bower) teams.

[Thomas Park](http://github.com/thomaspark) for inspiration via [Bootswatch](https://github.com/thomaspark/bootswatch/).

Copyright and License
---------------------
[BSD License](http://opensource.org/licenses/bsd-license.php)
&copy; 2013 Bradley Dunn
