# ScrapingNewsMongo

## Scrape echoJS News App
This application is a single page, full stack web app that scrapes and displays all stories from http://echoJS.com

Users are presented with a series of article headlines. Clicking on the link will give the user access to a link to display the entire article in a new tab; Clicking on the headline will enable user to add comments.

## Links
Heroku: [EchoJS scraper](https://secure-brook-41699.herokuapp.com/)

## Motivation
This project is a full-stack web app, using the Model-View-Controller(MVC) design pattern. It uses Mongo as persistent storage, and Mongoose as the modeling engine or ORM.

## File Overview — what does what?
This is a complex project. A short overview of the function and structure of each file will be helpful. We’ll look first at the file organization, then at the driver code, and then at how the MVC design pattern is implemented.

### Project Directory/File Structure

### Driver Code

* server.js
	* Requires the npm modules express, morgan, cheerio, axios and mongoose (to create the database connection and initialize the collections if not already present).	

server.js contains the code that retrieves the routes , does basic initialization, setup routes, and starts listening on the port 5000. Note that it also establishes for the Express server the /public directory as the source for static information (e.g., images and css).

### “Model” files
* models/articles.js.  Creates the model for the articles collection.
* models/note.js. Creates the model for the “notes” or “comments” collection.
* models/index.js export articles and notes models

## Tech/framework used
* Node
* Express
* Mongo
* Mongoose
* Cheerio
* MVC design pattern
* Css framework

## Features
This project is a complete, end-to-end implementation of a web app.
* Front End/Browser
	* CSS
	* Dynamic web page rendering
* Middleware
	* Express routing
* Server
	* Mongo Database