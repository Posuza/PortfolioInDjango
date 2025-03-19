
# Personal Portfolio Project

A Django-based personal portfolio website with blog functionality. This project allows you to showcase your work through a portfolio section and share your thoughts through a blog.

## Features

- **Portfolio Section**: Display your projects with images, descriptions, and links
- **Blog**: Share your thoughts and experiences with dated entries
- **Admin Panel**: Easily manage your portfolio projects and blog posts
- **Responsive Design**: Works on desktop and mobile devices

## Technology Stack

- Django 3.2
- Python 3
- HTML/CSS
- SQLite (default database)

## Project Structure

The project consists of two main Django apps:

1. **Portfolio App**: Manages the display of projects on the homepage
2. **Blog App**: Handles blog posts and their display

## Setup Instructions

### Prerequisites

- Python 3.x
- pip (Python package manager)

### Installation

1. Clone the repository
   ```
   git clone <repository-url>
   cd django3-personal-portfolio-main
   ```

2. Create a virtual environment (recommended)
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies
   ```
   pip install -r requirements.txt
   ```

4. Apply migrations
   ```
   python manage.py migrate
   ```

5. Create a superuser to access the admin panel
   ```
   python manage.py createsuperuser
   ```

6. Run the development server
   ```
   python manage.py runserver
   ```

7. Access the site at http://127.0.0.1:8000/

## Usage

### Adding Portfolio Projects

1. Log in to the admin panel at http://127.0.0.1:8000/admin/
2. Navigate to "Projects" under the Portfolio section
3. Click "Add Project" and fill in:
   - Title
   - Description
   - Image
   - URL (optional)

### Creating Blog Posts

1. Log in to the admin panel
2. Navigate to "Blogs" under the Blog section
3. Click "Add Blog" and fill in:
   - Title
   - Description
   - Date

## Customization

You can customize the project by:

1. Modifying templates in the `templates` directory
2. Adding CSS in the static files
3. Extending models to include additional fields

## Deployment

For production deployment:

1. Set `DEBUG = False` in settings.py
2. Configure a proper database (PostgreSQL recommended)
3. Set up static files serving
4. Use a production-ready web server like Gunicorn
5. Consider using Nginx as a reverse proxy
