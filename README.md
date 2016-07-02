# Electron MongoDB

Thick client demo app showing Electron and MongoDB working together.

This application can be run and built on Windows & OS X.  I've not tested it yet on Linux but it will build and run in Linux as well.

## Electron Links

Electron Home: http://electron.atom.io

Outstanding list of Electron links: https://github.com/sindresorhus/awesome-electron

Outstanding Electron blog post: http://www.toptal.com/javascript/electron-cross-platform-desktop-apps-easy

Full documentation on the electron-packager see: https://github.com/maxogden/electron-packager

NOTE:  To build Windows on Mac, follow the directions at the bottom of the electron-packager webpage.  I was unable to get "wine" installed correctly on my Mac at the time this was created.  I'll update when I'm able to build Windows on my Mac.

Outstanding Electron Video:  https://www.youtube.com/watch?v=OHOPSvTltPI

## MongoDB

Home Page: https://mongodb.github.io/node-mongodb-native/index.html

## Prerequisites

These prerequisites must be installed as described below.

- Install or have access to MongoDB.  You can use either an existing local MongoDB server or a remote MongoDB server.

	If you need one, install it and either start MongoDB or configure it to run automatically.  Please see the MongoDB documentation for your operating system. Please perform a test connection to your MongoDB server before proceeding.

	This application uses the default MongoDB connection string to connect to the test database that is installed automatically.

	Default connection string:	`mongodb://localhost:27017/test`

	If you are using a remote MongoDB server or you changed the default port on local install, you'll need to modify the above connection string.  The connection string is in the `/src/home/mongoService.js` file.


- Install node.js

- Install the Electron Prebuilt globally:

	`npm install -g electron-prebuilt`

## Download and Run

- Download the zip from this repo.
- Install root folder node modules.

	`cd / { path to app }`

	`npm install`


## Run the app

- From the app root folder

	`cd / { path to app }`

	`electron .`

	or

	`npm start`

## Results

The app will run and an alert dialog will advise you that the application has connected to MongoDB.

Presto, thick client.
