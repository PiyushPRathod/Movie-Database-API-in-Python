# Movie Database API in Python

This repository contains the resources and code for the course [Movie Database API in Python](https://www.educative.io/courses/movie-database-api-python) hosted on Educative.io.

## Course Overview

This course teaches how to build a movie database API using Python. By the end of the course, you'll have learned:

- How to use Python's Flask framework
- REST API concepts and implementation
- Integration of third-party services (like The Movie Database API)
- Handling requests and responses
- Managing databases using SQLAlchemy
- Best practices for error handling, testing, and more

## Contents

The repository is organized as follows:

- **/01-introduction-to-flask**: Learn the basics of Flask and set up a simple web server.
- **/02-creating-a-movie-api**: Step-by-step guide to creating a movie API using Flask.
- **/03-integrating-tmdb-api**: Integration of The Movie Database (TMDB) API to fetch movie data.
- **/04-database-setup-with-sqlalchemy**: Setting up and managing a database using SQLAlchemy.
- **/05-unit-testing-the-api**: Writing unit tests to ensure the reliability of the API.
- **/06-deployment**: How to deploy your Flask app to the cloud.

## Requirements

To run the code locally, you'll need:

- Python 3.7 or higher
- Flask 2.x
- SQLAlchemy
- Requests library
- TMDB API Key (you can sign up [here](https://www.themoviedb.org/signup))

### Installing dependencies

```bash
pip install -r requirements.txt
```

## Running the Project

1. **Clone this repository:**

   ```bash
   git clone https://github.com/yourusername/movie-database-api-python.git
   cd movie-database-api-python
   ```

2. **Install the dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

3. **Set your TMDB API Key as an environment variable:**

   ```bash
   export TMDB_API_KEY='your_tmdb_api_key'
   ```

4. **Run the Flask app:**

   ```bash
   python app.py
   ```

5. **Open your browser and navigate to http://127.0.0.1:5000 to see the running API.**

