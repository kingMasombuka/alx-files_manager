# Files Manager

This project is a compilation of back-end concepts: authentication, NodeJS, MongoDB, Redis, pagination and background processing.

The objective was to build a simple platform to upload and view files with:

- User authentication via a token
- List all files
- Upload a new file
- Change permission of a file
- View a file
- Generate thumbnails for images

|                                                                                                         |                                       ## Testing and Jobs

The project includes a queueing job system for generating thumbnails of images uploaded to the application. It also uses this feature to generate a welcome message when a new user is created. For all of this, Bull is used.

For testing of the application, Mocha is used in combination with Chai.

## Endpoints

The project performs all of its features through endpoints running in Express.

User endpoints are hosted in Redis, while files and user data is hosted in MongoDB.
