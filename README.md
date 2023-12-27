# Flask REST API First Project 💻

This project was designed to test my knowledge in these libraries and frameworks.</a>
Doing a CRUD in a network of stores, with different items, that can be included, updated or deleted.</a>

## What was used ⌨️

* Flask;
* Docker; 
* Flask-Smorest; 
* SQLAlchemy; 

## How to Test It 🖥️

- You will need a tool like Insomnia, to send requests to the API.
- The URL to send the requests is : (https://rest-apis-flask-python-project-x5j4.onrender.com)
- Replace the (url), with the url provided to test it properly.
- Replace the (id) with the generated id from previous requests.
- The first request may take a while (approximately 20 seconds), since the docker image is hosted in a free plan in render.com
- The key words to be passed are in the /models/item and /model/store

 ### Endpoints for Stores

 * POST= (url)/store - To create a new store - Key Word: name;
 * GET= (url)/store - For all store data;
 * GET= (url)/store/(id) - For receive a specific store data;
 * DELETE= (url)/store/(id) - For delete a specifc store;

 ### Endpoints for Items

 * POST= (url)/item - To create a new item - Key Word: name, price, store_id;
 * GET= (url)/item - For all item data;
 * GET= (url)/item/(id) - For receive a specific item data;
 * DELETE= (url)/store/(id) - For delete a specifc item;
 * PUT= (url)/item/(id) - To update a specific item, or create a new item if it was not found - Key Word: name, price, store_id;

## Work in Progress 🏗️

 This Rest API is in development, i want to add a differente type of database in the future such as PostgreSQL,also making a improvemente in the database relationships.
 Also, develop a user authentification for the endpoints.