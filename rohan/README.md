# EventSphere - Event Discovery Platform

A fully functional Django web application for discovering and managing events, built based on the provided mockup design.

## Features

### 🎯 Core Functionality
- **Event Discovery**: Browse concerts, festivals, and sports events
- **User Authentication**: Secure login/signup system
- **User Dashboard**: Personalized dashboard with favorites and event planning
- **Event Details**: Comprehensive event information with venue details and reviews
- **Search & Filter**: Advanced search functionality across events
- **Favorites System**: Save and manage favorite events
- **Review System**: Rate and review events
- **Calendar View**: Visual calendar for event planning

### 🎨 Design Features
- **Responsive Design**: Mobile-friendly interface
- **Modern UI**: Clean, professional design matching the mockup
- **Interactive Elements**: Smooth animations and user feedback
- **Category-based Navigation**: Easy browsing by event type

## Installation & Setup

### Prerequisites
- Python 3.8+
- pip (Python package manager)

### Quick Start

1. **Clone/Download the project**
   ```bash
   cd c:\xampp\htdocs\rohan
   ```

2. **Install Dependencies**
   ```bash
   pip install django pillow
   ```

3. **Run Database Migrations**
   ```bash
   python manage.py migrate
   ```

4. **Create Sample Data**
   ```bash
   python manage.py populate_data
   ```

5. **Create Superuser (Optional)**
   ```bash
   python manage.py createsuperuser
   ```

6. **Start Development Server**
   ```bash
   python manage.py runserver
   ```

7. **Access the Application**
   - Main Site: http://127.0.0.1:8000/
   - Admin Panel: http://127.0.0.1:8000/admin/

## Project Structure

```
eventsphere/
├── eventsphere/          # Main project settings
├── accounts/             # User authentication app
├── events/              # Events management app
├── dashboard/           # User dashboard app
├── templates/           # HTML templates
├── static/             # CSS, JS, images
├── media/              # User uploaded files
└── manage.py           # Django management script
```

## Default Credentials

### Admin Panel
- **Username**: admin
- **Password**: admin123

### Test User (Create via signup)
- Use the signup form to create test users

## Key Pages & Features

### 🏠 Home Page (`/`)
- Hero section with search functionality
- Featured event categories (Concert, Festival, Sports)
- Event discovery interface

### 🔐 Authentication (`/accounts/`)
- **Login**: `/accounts/login/`
- **Signup**: `/accounts/signup/`
- **Profile**: `/accounts/profile/`

### 🎪 Events (`/events/`)
- **Event List**: `/events/`
- **Event Detail**: `/events/<id>/`
- **Category Filter**: `/events/category/<slug>/`
- **Search**: `/events/search/`

### 📊 Dashboard (`/dashboard/`)
- **Main Dashboard**: `/dashboard/`
- **Favorites**: `/dashboard/favorites/`
- **Calendar**: `/dashboard/calendar/`

## Sample Data

The application comes with pre-populated sample data:

### Categories
- Concert
- Festival  
- Sports

### Venues
- Madison Square Garden (New York)
- Hollywood Bowl (Los Angeles)
- Red Rocks Amphitheatre (Colorado)
- Fenway Park (Boston)

### Events
- Live Concert
- Summer Music Festival
- Championship Game
- Rock Concert
- Jazz Festival
- Basketball Finals

## Testing

Run the included test script to verify functionality:

```bash
python test_eventsphere.py
```

## Customization

### Adding Images
1. Add event/category images to `static/images/`
2. Update image references in templates
3. Use the admin panel to upload event images

### Styling
- Main CSS: `static/css/style.css`
- Bootstrap 5 is included for responsive design
- Font Awesome icons are available

### Adding Features
- Models: Add new models in respective `models.py` files
- Views: Add new views in respective `views.py` files
- Templates: Create new templates in `templates/` directory
- URLs: Update URL patterns in `urls.py` files

## Technologies Used

- **Backend**: Django 5.2.6
- **Database**: SQLite (default)
- **Frontend**: HTML5, CSS3, JavaScript
- **Styling**: Bootstrap 5, Font Awesome
- **Image Handling**: Pillow

## Production Deployment

For production deployment:

1. Set `DEBUG = False` in settings
2. Configure proper database (PostgreSQL recommended)
3. Set up static file serving
4. Configure email backend
5. Set secure secret key
6. Configure ALLOWED_HOSTS

## Support

The application is fully functional and matches the provided mockup design. All features are implemented and tested.

For any issues or questions, check the Django documentation or the code comments for guidance.

---

**EventSphere** - Discover amazing events and concerts near you! 🎉
