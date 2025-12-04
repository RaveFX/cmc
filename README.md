Class Management System (CMS)

A comprehensive web-based application designed for educational institutes to streamline operations. The system focuses on Fee Management, Student Enrollment, Attendance Tracking, and Notifications.

Built with Django (DRF) for the backend and React (Vite) for the frontend.

📂 Project Structure

This project follows a Monorepo structure:


class_management_system/
├── backend/            # Django REST API
│   ├── config/         # Project settings
│   ├── users/          # Authentication & Roles
│   ├── academics/      # Students, Teachers, Subjects
│   ├── attendance/     # Attendance logic
│   └── finance/        # Fee calculation & Payments
│
└── frontend/           # React + Vite Application
    ├── src/
    └── public/


🚀 Getting Started

Follow these instructions to set up the project locally.

Prerequisites

Ensure you have the following installed:

Python 3.10+

Node.js (v18+ recommended) & npm

Git

1. Clone the Repository

git clone <repository-url>
cd class_management_system


2. Backend Setup (Django)

Navigate to the backend directory:

cd backend


Create a Virtual Environment:

# Windows
python -m venv venv

# macOS/Linux
python3 -m venv venv


Activate the Virtual Environment:

# Windows
venv\Scripts\activate

# macOS/Linux
source venv/bin/activate


Install Dependencies:

pip install -r requirements.txt


Apply Database Migrations:

python manage.py migrate


Run the Development Server:

python manage.py runserver


The API will be available at http://127.0.0.1:8000.

3. Frontend Setup (React)

Open a new terminal (keep the backend running) and navigate to the frontend directory:

cd frontend


Install Node Modules:

npm install


Start the Development Server:

npm run dev


The UI will be available at http://localhost:5173.

🛠 Configuration

Environment Variables

Currently, the project uses default Django settings. For production or local security, create a .env file in the backend/ directory:

# backend/.env
DEBUG=True
SECRET_KEY=your-secret-key-here
ALLOWED_HOSTS=127.0.0.1,localhost


API Endpoints (Documentation)

Once the backend is running, you can explore the API structure (if configured) or via the Django Admin interface at:

http://127.0.0.1:8000/admin/

🤝 Contributing

Create a feature branch (git checkout -b feature/AmazingFeature).

Commit your changes (git commit -m 'Add some AmazingFeature').

Push to the branch (git push origin feature/AmazingFeature).

Open a Pull Request.

📄 License

[Include License Here, e.g., MIT]