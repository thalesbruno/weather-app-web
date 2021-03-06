Weather app
===============
A weather application written in `node.js` that gets from [mapbox.com](mapbox.com) the geocode location of your searched place, and use it to request from  [darksky.net](darksky.net) a forecast summary report of that location. Accessible at [https://thlsbrn-weather-app.herokuapp.com](https://thlsbrn-weather-app.herokuapp.com).

<!--ts-->
Table of contents
-----------------
* [Installation and Usage](#installation-and-usage)
* [Technologies covered](#technologies-covered)
  * [Express](#express)
  * [HBS](#hbs)
  * [Heroku](#heroku)

<!--te-->
Installation and Usage
======================

Clone repository  
```bash
git clone https://github.com/thalesbruno/weather-app-web
```

On brand new weather-app-web directory created, run `npm install` to install all project dependencies.  

So, you'll be already able to start the app using `node src/app.js`.  


Technologies covered
====================

Express
-------
>Express is a web framework for node.

Install  
```bash
npm i express
```

Usage  
```javascript
const express = require('express')
const app = express()

app.get('', (req, res) => {
  res.send('Hello World')
})

app.listen(3000, () => {
  console.log('Server listening on port 3000')
})
```

:page_facing_up: [Read the docs](https://expressjs.com/en/4x/api.html)

HBS
---
>Express.js view engine for handlebars.js

Install  
```bash
npm install hbs
```

Usage  
```javascript
app.set('view engine', 'hbs')
```

:page_facing_up: [Read the docs](https://www.npmjs.com/package/hbs)

Heroku
------
>Heroku is a cloud platform that lets companies build, deliver, monitor and scale apps

Install  
:page_facing_up: [How to install Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli)

Login into heroku from heroku local cli:  
`heroku login`

Passing ssh keys for make things secure:  
`heroku keys:add`

Creating the app name. The name must be unique in all heroku base:  
`heroku create heroku-unique-app-name`

:page_facing_up: [Read the docs](https://devcenter.heroku.com/categories/reference)
