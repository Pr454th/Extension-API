This project is an API used by a Firefox extension to set and get created notes. The API is built using Node.js and utilizes the Express framework.

## Getting Started

To get started with the project, follow these steps:

1. Clone the repository onto your local machine using `git clone <repository_url>`
2. Run `npm install` to install all dependencies required for the project.
3. Create a `.env` file in the root directory and specify the environment variables `PORT` (the port number for the server to listen on) and `MONGO_URL` (the URI for the MongoDB database to use).
4. Run `npm start` to start the server.

## API Endpoints

The following endpoints are available in the API:

### POST /setnote

Creates a new note in the database. The request body should contain a JSON object with a `id` and `note` field.The note will be automatically deleted after 20 minutes.

### GET /getnote/:id

Retrieves a specific note with the given `id` from the database.

### Dependencies

The project uses the following dependencies:

* `express`: web application framework
* `mongoose`: MongoDB object modeling tool
* `dotenv`: loads environment variables from a .env file
* `cors`: enables Cross-Origin Resource Sharing (CORS)

## Contributing

We welcome contributions from the community! Please refer to the CONTRIBUTING.md file in the repository for more information on how to contribute to the project.

## License

The project is licensed under the MIT License. See the LICENSE file in the repository for more information.
