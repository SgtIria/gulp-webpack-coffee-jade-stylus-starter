gulp-webpack-coffee-jade-stylus-starter
=======================================

Took me a day to figure out how this stuff works.. in case others are interested

Based on https://github.com/johnthethird/react-starter-template

This is so I can use stylus and jade, which are awesome with livereload. Can modify the whole DOM with the flick of a single line in vim (how it should be).

This is also so I can use browserify-ish stuff at la webpack. I love substack's work/philosophy/everything, but webpack just works for requiring jade files from within coffeescript.

This is also allows me to use coffeescript. Again, things kind of breakdown and are hard to hack if you have require jade IN the coffeescript. And I am resisting reading more about how to figure that out... I was able to get it to work with webpack without gulp and then I just switched to webpack.

See that entryJade gulp task? That's because I have jade files that house the entry point into the rest of the browserify/webpack bundle. So I need those too.

Customize all you want. Seems good enough. And I can finally require('./something.jade') in coffeescript. I've been grinding on that my whole life these past 24 hours, having only recently gotten back into FE development. 

Some links:

https://github.com/tooling/book-of-modern-frontend-tooling
http://gulpjs.com/
https://github.com/johnthethird/react-starter-template

Oh, btw I use nvm and I most definitely 'use v.11.12'. v.11.13 has problems. And I think React is cool:

https://github.com/eggheadio/egghead-react-flux-example

I'm just not quite ready for it yet.

## If you're like me and are just re-starting-out

```sh
install node
nvm install 0.11.12
nvm use 0.11.12
npm install -g nvm
npm install -g gulp
git clone https://github.com/tmsh/gulp-webpack-coffee-jade-stylus-starter.git
cd gulp-webpack-coffee-jade-stylus-starter
npm install
gulp dev
```
