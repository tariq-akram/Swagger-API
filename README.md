# FastAPI User API

This FastAPI project provides a simple API for managing user data. It includes endpoints for creating, retrieving, updating, and deleting user records.

## Installation

1. Clone this repository:

    ```bash
    git clone https://github.com/your-username/fastapi-user-api.git
    cd fastapi-user-api
    ```

2. Create a virtual environment (optional but recommended):

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

3. Install the required dependencies:

    ```bash
    pip install -r requirements.txt
    ```

## Configuration

1. Configure your database connection in `config/db.py`. Replace the placeholder values with your actual database credentials.

2. Make sure you have MongoDB installed and running.

## Usage

1. Run the FastAPI app:

    ```bash
    uvicorn index:app --reload
    ```

2. Access the Swagger documentation at `http://localhost:8000/docs` to explore the available endpoints.

## Endpoints

### GET /users/

Returns a list of all users.

### GET /users/{id}

Returns details of a specific user by ID.

### POST /users/

Creates a new user. Send a JSON payload with user data.

### PUT /users/{id}

Updates an existing user by ID. Send a JSON payload with updated user data.

### DELETE /users/{id}

Deletes a user by ID.

## Models

The `User` model is defined in `models/user.py`. Customize it according to your requirements.

## Contributing

Feel free to contribute to this project by opening issues or submitting pull requests. Let's make it better together!
