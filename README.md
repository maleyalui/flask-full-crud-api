# Event Management
  A simple Flask REST API for managing events. This project allows you to create, update, and delete events using standard HTTP methods with JSON data. It uses an in-memory list to simulate a database.
  
 ## Features
    POST /events – Add a new event
    PATCH /events/<id> – Update the title of an existing event
    DELETE /events/<id> – Remove an event from the list
    Returns structured JSON with proper HTTP status codes
    Error handling for invalid requests (missing title, non-existent event)

 ## How it works
    ```bash
    git clone <your-repo-url>
    cd flask-full-crud-api
    ```

 ## Create a virtual enviroment:
    ```bash
    python -m venv venv
    source venv/bin/activate
    ```

 ## Install dependancies:
    ```bash
    pip install flask
    ```

 ## Run the Flask server:
    ```bash
    python app.py
    ```

 ## Examples
   ### Create Event (POST):
      ```bash
      POST /events
      Content-Type: application/json

      {
      "title": "Hackathon"
      }
      ```

   ### Update Event(PATCH):
      ```bash
          PATCH /events/1
          Content-Type: application/json

          {
          "title": "Hackathon 2025"
          }
      ```

   ### Delete Event(DELETE):
      ```bash
      DELETE /events/2
      ```

 ## Contributors
    Luis Maleya
