# SmartBrain-api - Dockerized
Final project for ZTM course - using Docker

1. Clone this repo
2. run `npm install`
3. Make sure you have docker installed and running on your computer
4. Run `docker-compose up` ( you may have to run `docker-compose up --build` for the first setup phase)
4. You must add your own API key in the `controllers/image.js` file to connect to Clarifai API.
5. You will also need to update Line 22 in server.js to your client app port (i.e. 3001)

**Important:** if you are getting conflict erros, you should run `docker stop <container name>` that is already running in the background.
**Important:** if you are getting other erros, you should run `docker-compose down` to bring everything down, and start over.

To access backend's bash:
Run `docker-compose exec smart-brain-api bash`

To access postgres: (adjust PORT number if needed)
Run  `psql postgres://<username>:<password>@localhost:5432/smart-brain`

To access redis:
Run `docker-compose exec redis redis-cli`

You can grab Clarifai API key [here](https://www.clarifai.com/)

** Make sure you use postgreSQL instead of mySQL for this code base.

