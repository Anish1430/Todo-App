# Todo App

This is a simple Todo application built with Spring Boot.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Setup](#setup)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Models](#models)
- [Controllers](#controllers)
- [Configuration](#configuration)
- [Running the Application](#running-the-application)

## Introduction
This project is a simple Todo application built using Spring Boot. It allows users to create, read, update, and delete tasks.

## Features
- Create a new Todo
- Get all Todos
- Update the status of a Todo
- Delete a Todo
- Get all undone Todos
- Remove multiple Todos by IDs

## Setup
1. Ensure you have Java and Maven installed.
2. Clone this repository.

## Usage
1. Build the project using Maven.
2. Run the application.

## API Endpoints
- **Create a Todo**
  - `POST /Creatingtodo`
  - Add a new Todo to the list.

- **Get all Todos**
  - `GET /todos`
  - Retrieve a list of all Todos.

- **Update Todo Status**
  - `PUT /todo/id/{id}/status`
  - Update the status of a Todo by providing its ID.

- **Delete a Todo**
  - `DELETE /todo/id/{id}`
  - Remove a Todo by its ID.

- **Get all undone Todos**
  - `GET /todos/unDone`
  - Retrieve a list of all undone Todos.

- **Remove multiple Todos by IDs**
  - `DELETE /todos/ids`
  - Remove multiple Todos by providing a list of their IDs.

## Models
### Todo
- `todoId`: Integer
- `todoName`: String
- `todoStatus`: boolean

## Controllers
### TodoController
- Manages all the Todo related API endpoints.

## Configuration
### BeanBag
- Configuration class that defines a `List<Todo>` as a Bean.

## Running the Application
1. Set the server port to 8082 in your `application.properties` file.
