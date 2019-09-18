# Installing dependencies and running the project:

# Required tools
- Python3
- pip3
- Postgres
- npm

# Installing Dependencies
- python3 -m venv venv (create a virtual env folder called venv)
- source venv/bin/activate (this activates the virtual environment)
- pip3 install -r requirements.txt (install all of the dependencies in the requirements.txt into venv)

## Make sure you have activated the virtual env to ensure flask commands run properly:

# Setting up your environment variables
- You must create a file in the root directory of the project called .env with the following variables set:
    FLASK_APP=app
    FLASK_ENV=development
    DATABASE_URL=postgresql://loki:00000000@project9900-v2-sdyney.clnpnedcibyx.ap-southeast-2.rds.amazonaws.com:5433/loki
- When the application starts, it will load the environment variables by reading in the file created above.

# Running Flask application (backend)
- flask run (this only works correctly if you have your environment variables defined as described in the previous step above)

# Running Vue.js application (frontend)
- cd frontend/
- npm install (install dependencies)
- npm start (build and start frontend)

At this point, you should have both the Flask and Vue.js application running. You can now navigate to http://localhost:8080 in your browser to see the application.