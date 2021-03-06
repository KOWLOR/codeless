<img src="https://raw.githubusercontent.com/flexbox/codeless/master/source/assets/images/codeless-middleman.jpg" alt="Middleman advanced template" align="center" />
<br />

<div align="center"><strong>Start your next Middleman project in seconds</strong></div>
<div align="center">A highly scalable, rails ready foundation with the best DX and a focus on SEO & best practices.</div>
<br />
<div align="center">

<a href="https://travis-ci.org/flexbox/codeless">
  <img src="https://travis-ci.org/flexbox/codeless.svg?branch=master" alt="Build Status">
</a>
</div>
<br />

###### Preprocessing
- [Slim](http://slim-lang.com) *[for html]*
- [Sass](http://sass-lang.com) *[for css]*
- [CoffeeScript](http://coffeescript.org) *[for js]*

###### Tools
- [Yarn](https://yarnpkg.com) *[package management]*
- ~~[Bower](http://bower.io) *[package management]*~~
- [GitHub Pages](http://pages.github.com) *[deployment/hosting]*
- [Middleman Autoprefixer](https://github.com/middleman/middleman-autoprefixer) *[Automatically add vendor prefixes to CSS rules]*
- [Middleman Favicon Maker](https://github.com/follmann/middleman-favicon-maker) *[Generate favicon files in various sizes]*
- [Middleman Live Reload](https://github.com/middleman/middleman-livereload) *[Reloads the page when files change]*

## Getting Started

Install Middleman

    $ gem install middleman

Start your project

    $ cd ~/path/to/your/project
    $ middleman init awesome-project --template=flexbox/codeless
    
:warning: This project is not __Middleman 4 ready__, due to nightmare dependency with `middleman-deploy`.
    
### Dependencies

You need [Bundler](http://bundler.io/) to install gems

    $ gem install bundler

Then, install them

    $ bundle install

### Yarn

Find and install the packages you need…

    $ yarn search package-name
    $ yarn add package-name
    
If the project already contains [Yarn](https://yarnpkg.com) dependencies, run

    $ yarn

###### css files

    @import 'folder/file'

###### js files

    #=require 'folder/file'


### Architecture

Stylesheets, fonts, images, and JavaScript files go in the `/source/assets/` directory.
Vendor stylesheets and JavaScripts should go in each of their `/bower_components/` directories.

    codeless/
    ├── node_modules/
    │    └── ...
    ├── source/
    │   ├── assets/
    │   └── ...

### Browser preview

    middleman server

### Deploying to GitHub Pages

    middleman build
    middleman deploy
    
Note :
- If you get an error with `middleman build`, make sure [Imagemagik](http://www.imagemagick.org/script/index.php) is installed `brew install imagemagick`
- If you deploy on Github pages, don't forget to uncomment these two lines in `config.rb` :

    activate :relative_assets
    set :relative_links, true

## Author

| [![twitter/_flexbox](https://gravatar.com/avatar/66ecc55f1bc2e5863eb516ee6f20794e?s=70)](https://twitter.com/_flexbox "Follow @_flexbox on Twitter") |
|---|
| [David Leuliette](http://davidl.fr/) |

## License

This project is free software, and may be redistributed under [GNU/GPL license](LICENSE.md).
