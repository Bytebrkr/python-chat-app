# Chat Application Readme
This is a simple chat application built with Flask and Flask-SocketIO. It allows users to create or join chat rooms and engage in real-time messaging with other users in the same room.

## Setup Instructions
To set up and run the application, follow these steps:

Clone the Repository: Clone this repository to your local machine using Git.

Install Dependencies: Navigate into the project directory and install the required Python dependencies

python app.py

Access the Application: Once the application is running, open your web browser and navigate to http://localhost:5000 to access the chat application.

## Usage
## Home Page
Upon accessing the application, you will be directed to the home page where you can enter your name and either join an existing room or create a new one.
If you choose to join an existing room, you need to enter the room code.
If you choose to create a new room, a unique room code will be generated for you.
## Chat Room
Once you enter a room, you can start sending and receiving messages in real-time.
All messages sent within the room will be displayed to all participants.
You can see a list of previous messages when you enter a room.
Socket Events
The application utilizes Flask-SocketIO for real-time communication. It handles the following socket events:

message: When a user sends a message, it is broadcasted to all participants in the room.
connect: When a user connects to the server, they are added to the room and a notification is sent to other participants.
disconnect: When a user disconnects from the server, they are removed from the room and a notification is sent to other participants.

## Dependencies
The main dependencies used in this project are:

Flask: A lightweight WSGI web application framework in Python.
Flask-SocketIO: Provides Flask integration with Socket.IO, enabling real-time bidirectional communication between web clients and the server.
Random: Python standard library module for generating random numbers and data.
String: Python standard library module for handling string operations.


## Future updates- using aws?

Elastic Beanstalk- you can access your Flask application using the URL provided by Elasict Elastic Beanstalk.
