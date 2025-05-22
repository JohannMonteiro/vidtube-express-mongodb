
# VidTube
================

A project inspired by YouTube, built with Node.js, Express, and MongoDB.

## Table of Contents
-----------------

- [VidTube](#vidtube)
  - [Table of Contents](#table-of-contents)
  - [Features](#features)
  - [Installation](#installation)
  - [Usage](#usage)
  - [API Documentation](#api-documentation)
    - [Endpoints](#endpoints)
  - [Models](#models)
  - [Controllers](#controllers)
  - [Middlewares](#middlewares)
  - [Utils](#utils)

## Features
------------

* User registration and login
* Video upload and streaming
* Commenting and liking system
* User profiles and channels
* Watch history and subscriptions

## Installation
------------

To install the project, run the following command:

```bash
npm install
```

## Usage
-----

To start the server, run the following command:

```bash
npm start
```

The server will start on port 8001. You can access the API endpoints by visiting `http://localhost:8001/api/v1/` in your web browser.

## API Documentation
-----------------

The API documentation is available at `http://localhost:8001/api/v1/docs`.

### Endpoints

* **Users**
	+ `POST /users/register`: Register a new user
	+ `POST /users/login`: Login a user
	+ `GET /users/current`: Get the current user
	+ `GET /users/:username`: Get a user by username
* **Videos**
	+ `POST /videos/upload`: Upload a new video
	+ `GET /videos/:id`: Get a video by ID
	+ `GET /videos`: Get all videos
* **Comments**
	+ `POST /comments/create`: Create a new comment
	+ `GET /comments/:id`: Get a comment by ID
	+ `GET /comments`: Get all comments
* **Likes**
	+ `POST /likes/create`: Create a new like
	+ `GET /likes/:id`: Get a like by ID
	+ `GET /likes`: Get all likes

## Models
---------

The project uses the following models:

* **User**: Represents a user in the database
* **Video**: Represents a video in the database
* **Comment**: Represents a comment in the database
* **Like**: Represents a like in the database

## Controllers
-------------

The project uses the following controllers:

* **UserController**: Handles user-related requests
* **VideoController**: Handles video-related requests
* **CommentController**: Handles comment-related requests
* **LikeController**: Handles like-related requests

## Middlewares
-------------

The project uses the following middlewares:

* **AuthMiddleware**: Handles authentication and authorization
* **ErrorMiddleware**: Handles errors and exceptions

## Utils
--------

The project uses the following utils:

* **ApiResponse**: Represents a response from the API
* **ApiError**: Represents an error from the API
* **asyncHandler**: Handles asynchronous requests
* **cloudinary**: Handles cloudinary uploads and deletions
