# Audiobook App

A full-stack audiobook application built with Django (backend) and Flutter (frontend). This app allows users to browse, search, and review audiobooks.

## Features

- Browse and search audiobooks
- View detailed audiobook information like title,author,genre,description,cover image and average rating
- Add, edit, and delete reviews for audiobooks
- Add,edit and delete audiobooks information
- Filter audiobooks by genre and author name
- Sort audiobooks by rating
- Responsive design for web and mobile platforms

## Tech Stack

### Backend
- Django 3.2+
- Django REST Framework 3.12+
- MySQL 8.0+

### Frontend
- Flutter 2.5+
- Provider for state management
- http package for API requests

## Dependencies

### Backend Dependencies
- asgiref==3.4.1
- Django==3.2.9
- djangorestframework==3.12.4
- mysqlclient==2.1.0
- pytz==2021.3
- sqlparse==0.4.2
- django-cors-headers==3.10.0

### Frontend Dependencies
- flutter_sdk: ">=2.12.0 <3.0.0"
- provider: ^6.0.0
- http: ^0.13.3

## Setup and Installation

### Backend Setup

1. Clone the repository:
git clone https://github.com/your-username/audiobook_app.git
cd audiobook_app/backend


2. Create a virtual environment and activate it:
python -m venv venv
source venv/bin/activate  # On Windows, use venv\Scripts\activate


3. Install the required packages:
pip install -r requirements.txt


4. Set up the MySQL database:
   - Create a new MySQL database for the project
   - Update the `DATABASES` configuration in `settings.py`:
     ```
DATABASES = {
'default': {
'ENGINE': 'django.db.backends.mysql',
'NAME': 'your_database_name',
'USER': 'your_mysql_username',
'PASSWORD': 'your_mysql_password',
'HOST': 'localhost',
'PORT': '3306',
}
}


5. Run migrations:
python manage.py makemigrations
python manage.py migrate


7. Create a superuser:
python manage.py createsuperuser


8. Start the development server:
python manage.py runserver


The backend should now be running at `http://localhost:8000`.

### Frontend Setup

1. Navigate to the frontend directory:
cd ../frontend


2. Ensure you have Flutter installed and set up. If not, follow the [official Flutter installation guide](https://flutter.dev/docs/get-started/install).

3. Get the Flutter packages:
flutter pub get


4. Run the app:
flutter run -d chrome  # For web

or
flutter run  # For mobile emulator


## API Endpoints

- `GET /api/audiobooks/`: List all audiobooks
- `POST /api/audiobooks/`: Create a new audiobook
- `GET /api/audiobooks/{id}/`: Retrieve a specific audiobook
- `PUT /api/audiobooks/{id}/`: Update a specific audiobook
- `DELETE /api/audiobooks/{id}/`: Delete a specific audiobook
- `GET /api/reviews/`: List all reviews
- `POST /api/reviews/`: Create a new review
- `GET /api/reviews/{id}/`: Retrieve a specific review
- `PUT /api/reviews/{id}/`: Update a specific review
- `DELETE /api/reviews/{id}/`: Delete a specific review

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request


## Acknowledgments

- [Django Documentation](https://docs.djangoproject.com/)
- [Django REST Framework Documentation](https://www.django-rest-framework.org/)
- [Flutter Documentation](https://flutter.dev/docs)
- [Provider Package](https://pub.dev/packages/provider)
- [MySQL Documentation](https://dev.mysql.com/doc/)
## Contact

Jay Dutonde - jaydutonde12@gmail.com
      
