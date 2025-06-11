
# Fitness Studio Booking System

A simple Django-based booking system for a fictional fitness studio. Users can view available classes, book them, and cancel bookings.

---

## Features

- View upcoming fitness classes
- Book a class
- Cancel a booking
- Track bookings by email
- Timezone-aware class times

---

## Tech Stack

- Python 3
- Django (no REST Framework)
- SQLite (default in-memory or file-based DB)
- HTML (basic templates)

---

## Setup Instructions

1. **Clone the repository** (or unzip):
   ```bash
   git clone https://github.com/chebrolusrikanth/Booking-API-.git
   cd fitness-booking
   ```

2. **Create a virtual environment**:
   ```bash
   python -m venv venv
   source venv/bin/activate 
   ```

3. **Install Django**:
   ```bash
   pip install django
   ```

4. **Run migrations**:
   ```bash
   python manage.py migrate
   ```

5. **Load seed data (optional)**:
   ```bash
   python manage.py loaddata seed_data.json
   ```

6. **Run the server**:
   ```bash
   python manage.py runserver
   ```

7. **Access the app** at:
   ```
   http://127.0.0.1:8000/
   ```

---

## Sample cURL Requests

### Book a class:
```bash
curl -X POST http://127.0.0.1:8000/book/ -d "class_id=1&client_name=John Doe&client_email=john@example.com"
```

### View bookings:
Use the form at `/view-bookings/` and enter your email.

---

## Seed Data

This will load 3 fitness classes:
- Yoga
- Zumba
- HIIT

All scheduled within the next week.

---

## Loom Video

Link : https://www.loom.com/share/f5ae0e12b5b04226bb5f60658f5676d8?sid=df1ca2b7-6272-4813-9763-18f76034a49f

---

## Author

- Chebrolu Bala Sai Srikanth
