## weather-rest-api-node

#### Technologies

- Node.js
- Express.js
- Typescript
- Redis
- MongoDB
- OpenWeatherMap's API
- Mocha

#### Prerequisite

To build and run this app locally you will need a few things:

- Install Node.js
- Install MongoDB
- Install VS Code

#### How to run

To run this application, you have to set your own MongoDB Atlas connection string and OpenWeatherAPI app id in environmental variables after that follow the bellow steps.

- git clone https://github.com/bhavinsa/weather-rest-api.git
- cd weather-rest-api
- npm install

.env file - add the APP_ID & MONGO_URI

    PORT = 5000
    MONGO_URI = mongodb://localhost:27017/?readPreference=primary&appname=MongoDB%20Compass&ssl=false
    REDIS_PORT = 6379
    REDIS_HOST = localhost
    REDIS_CACHE_TIMEOUT  = 120
    NODE_ENV=Developement
    WEATHER_API = https://api.openweathermap.org/data/2.5/weather
    APP_ID=

- npm run dev
- npm run test
- npm run build - for production

🚀 Features

- > Get weather information of a city from OPenWeatherAPI and store it in MongoDB
- > Open browser and hit url - http://localhost:5000/api/v1/vopak/weathers/?city=ahmedabad
- > Get list of weathers of present date
- > Get weather of a specific city of present date
- > GET average tempreture of a location based on for a given month of the year
