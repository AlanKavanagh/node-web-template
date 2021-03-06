A Node.js web-app template ready for you! (SEO friendly)
=========

This is an empty template for you to start off your web applicatoin. All the stuff used in this project are chosen carefully with an outstanding exprience of building webb-apps.

This template is ready to run on Heroku! You can find a **demo** running on Heroku here: http://node-web-template.herokuapp.com/

###Tech Stack Included
- **Express** *as web framework* | http://expressjs.com
- **CoffeeScript** *instead of JavaScript* | http://coffeescript.org
- **Dust.js** *as templating language (LinkedIn fork)* | http://linkedin.github.io/dustjs
- **LESS** *in support of CSS* | http://www.lesscss.org
- **Backbone.js** *as client-side MVC* | http://backbonejs.org
- **CoffeeLint** *as style checker* | http://www.coffeelint.org
- **MongoDB** *as database (obviously)* | http://www.mongodb.org
- **Moongoose** *as object modelling for MongoDB* | http://mongoosejs.com
- **Konfig** *as config manager and parser* | https://github.com/vngrs/konfig/

###What you will find inside
- One template to rule them all: Use one template for front/back end
- SEO friendly Backbone.js: First page rendering happens on the server side
- Pretty fast and async rendering of pages, thanks to Dust.js
- CoffeeScript and LESS is already in place
- Test ready: various sample tests are there for you
- Asset pipelining
- Ready to run on Heroku straight away (if MongoDB available)
- A simple structure for Heroku Scheduled Jobs
- Sample models and schema for Moongoose
- and more...

--------------------------
##Why Dust.js
To be able to answer 'Why', we should answer 'What is Dust.JS'. **Dust.JS is a JavaScript templating engine.** It is designed to provide a clean separation between presentation and logic without sacrificing ease of use.

Dust templates are compiled into JavaScript and will work at both browser-side and server-side. In our case, this enables us to use same template file for generating pages at server-side and Backbone powered browser-side. You should be asking yourself: 'Why I need this?". The answer is straight forward: 
- Same template file for server and browser side.
- One file to maintain, fix and make changes.

####Why we generate templates at server-side
We use Backbone, so why we want to render pages at server-side? First of all we only render first page loads at the server. **Since we want a SEO-friendly website**, we need first page loads generated by server-side so they will be avaible for web spiders (which does not execute JavaScript). Backbone comes into play after first page load. When user clicks a link after first page load, next page is rendered with JavaScript using Backbone.

**Why not a Phantom.JS like solutions for this?** This kind of solution means you use headless-browser or libraries to render your page/JS as an user, and then serve it's rendered output. This has some disadvantages:
- Adds extra software layer and complexity
- Hard to inspect problems
- These solutions provided for testing needs

**Dust.JS among other templating engines** 
There are lots of templating engines, and some of them are great! But the reasons why we chose are pretty solid, these are:
- Performance
- Features
- Flexibility
- Logic-less
- Easy to use
- Good documentation
- And more (you can find more in the following readings)

To get more familiar about the choice of Dust.JS, please have a look at these readings:
- [Templating throwdown](http://engineering.linkedin.com/frontend/client-side-templating-throwdown-mustache-handlebars-dustjs-and-more)
- [{Dust.js} at Linked.in slides](http://www.slideshare.net/brikis98/dustjs)
- [Leaving JSP in the dust](http://engineering.linkedin.com/frontend/leaving-jsps-dust-moving-linkedin-dustjs-client-side-templates)
