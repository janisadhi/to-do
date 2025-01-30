# To-Do App

A simple and visually appealing to-do list application built using Flask and SQLite, featuring a modern UI with Tailwind CSS.

## Features
- Add, delete, and mark tasks as completed
- Uses Flask as the backend framework
- SQLite for lightweight database management
- Tailwind CSS for a beautiful and responsive UI
- Runs on `0.0.0.0` for accessibility in a production environment

## Installation
### Prerequisites
- Python 3.x
- pip (Python package manager)

### Setup
1. Clone the repository:
   ```sh
   git clone https://github.com/janisadhi/to-do.git
   cd todo_app
   ```
2. Create a virtual environment (optional but recommended):
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```
3. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
4. Run the application:
   ```sh
   python app.py
   ```
5. Open the application in a browser:
   - Go to `http://127.0.0.1:5000/` (for local use)
   - Or access via server IP if deployed

## Deployment
For deploying to a production environment, consider using:
- Gunicorn for running the Flask app
- Nginx as a reverse proxy
- Docker for containerization

### Docker Deployment
1. Build the Docker image:
   ```sh
   docker build -t todo-app .
   ```
2. Run the container:
   ```sh
   docker run -d -p 5000:5000 --name todo-container todo-app
   ```
3. Open the application in a browser:
   - Go to `http://127.0.0.1:5000/` (for local use)
   - Or access via server IP if deployed

Example with Gunicorn:
For deploying to a production environment, consider using:
- Gunicorn for running the Flask app
- Nginx as a reverse proxy
- Docker for containerization

Example with Gunicorn:
```sh
pip install gunicorn
gunicorn -w 4 -b 0.0.0.0:5000 app:app
```

## License
This project is open-source and free to use.

