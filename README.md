# Notes App

A simple Notes application built using Django for the backend and React for the frontend. This project is designed to help you learn and integrate Django and React seamlessly.

---

## Features

- User Authentication (Login/Logout/Register)
- CRUD operations for notes
- Responsive user interface with React
- RESTful API powered by Django REST framework

---

## Technology Stack

### Backend
- **Django**: Web framework for Python
- **Django REST Framework**: For creating APIs
- **SQLite**: Default database for Django (Can be replaced with PostgreSQL/MySQL)

### Frontend
- **React**: JavaScript library for building user interfaces
- **Axios**: For making HTTP requests

---

## Setup Instructions

### Prerequisites

Ensure you have the following installed:
- Python (>= 3.8)
- Node.js (>= 16)
- npm or yarn
- Git

### Clone the Repository
```bash
$ git clone https://github.com/<your-username>/<your-repo>.git
$ cd <your-repo>
```

### Backend Setup

1. Navigate to the backend directory:
   ```bash
   $ cd backend
   ```

2. Create and activate a virtual environment:
   ```bash
   $ python -m venv venv
   $ source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   $ pip install -r requirements.txt
   ```

4. Apply migrations and run the server:
   ```bash
   $ python manage.py makemigrations
   $ python manage.py migrate
   $ python manage.py runserver
   ```

### Frontend Setup

1. Navigate to the frontend directory:
   ```bash
   $ cd ../frontend
   ```

2. Install dependencies:
   ```bash
   $ npm install
   ```

3. Start the development server:
   ```bash
   $ npm run dev
   ```

### Access the Application

- Backend API: [http://127.0.0.1:8000/](http://127.0.0.1:8000/)
- Frontend: [http://localhost:5173/](http://localhost:5173/)

---

## Project Structure

```
<your-repo>/
├── backend/
│   ├── manage.py
│   ├── backend/
│   │   ├── settings.py
│   │   ├── urls.py
│   │   └── ...
│   ├── notes/
│   │   ├── models.py
│   │   ├── views.py
│   │   ├── serializers.py
│   │   └── ...
│   └── ...
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   └── App.js
│   ├── public/
│   └── ...
├── README.md
└── ...
```

---

## API Endpoints

### Authentication
- `POST /api/token/`: Obtain JWT token
- `POST /api/token/refresh/`: Refresh JWT token

### Notes
- `GET /api/notes/`: List all notes
- `POST /api/notes/`: Create a new note
- `GET /api/notes/<id>/`: Retrieve a specific note
- `PUT /api/notes/<id>/`: Update a note
- `DELETE /api/notes/<id>/`: Delete a note

---

## Contributing

1. Fork the repository
2. Create a new branch (`git checkout -b feature-name`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature-name`)
5. Open a Pull Request

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgments

- Django and React documentation
- Tutorials and community resources

---

## Contact

Feel free to reach out via GitHub issues if you encounter any issues or have suggestions.
