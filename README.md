# Flask REST API First Project 💻

This project was designed to test my knowledge in these libraries and frameworks.
Doing a CRUD in a network of stores, with different items, that can be included, updated or deleted, also with tags, that are related with the stores.
Also using JWT to user athentification, for more secure requests

## What was used ⌨️

* Flask;
* Docker; 
* Flask-Smorest; 
* SQLAlchemy; 

## How to Test It 🖥️

- You will need a tool like Insomnia, to send requests to the API.
- The URL to send the requests is : (https://rest-api-flask-python-project-21bq.onrender.com)
- Replace the (url), with the url provided to test it properly.
- Replace the (id) with the generated id from previous requests.
- The first request may take a while (approximately 20 seconds), since the docker image is hosted in a free plan in render.com

 ### Endpoints for User

 * POST= (url)/register - To create a new User - Key Words: username, password;
 * POST= (url)/login - To login and generate access tokens and refresh tokens - Key Words: username, password;
 * POST= (url)/logout - To put a user in the block list, and revoke the tokens - - Key Words: username, password;
 * POST= (url)/refresh - To get a non-fresh token;
 * GET= (url)/user/(id) - To get informations of a user;
 * DELETE= (url)/user/(id) - To delete a user;

### Endpoints for Tags
The ID in (url)/store are the IDs of a store created previously.

 * POST= (url)/store/(id)/tag - To create a tag and connect it to a store - Key Words: name,
 * GET= (url)/tags/(id) - To get informations of a specific tag;
 * GET= (url)/store/(id)/tag - To get all tags related with a store;
 * DELETE= (url)/(id) - To delete a specific tag.


 ### Endpoints for Stores

 * GET= (url)/store - For all store data;
 * GET= (url)/store/(id) - For receive a specific store data;
 * POST= (url)/store - To create a new store - Key Word: name;
 * DELETE= (url)/store/(id) - For delete a specifc store;

 ### Endpoints for Items

 * GET= (url)/item - For all item data;
 * GET= (url)/item/(id) - For receive a specific item data;
 * POST= (url)/item - To create a new item - Key Word: name, price, store_id;
 * DELETE= (url)/store/(id) - For delete a specifc item;
 * PUT= (url)/item/(id) - To update a specific item, or create a new item if it was not found - Key Word: name, price, store_id;
