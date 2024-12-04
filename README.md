# Event Landing Page

A modern, responsive event landing page built with Flask, featuring registration forms, interactive maps, and email integration.

## Features

- Responsive design using CSS Grid and Flexbox
- User registration with email confirmation
- Interactive Google Maps integration
- Contact form with backend processing
- Modern animations and transitions
- Mobile-friendly layout

## Prerequisites

- Python 3.8+
- pip (Python package manager)
- A Gmail account for sending emails
- Google Maps API key

## Setup

1. Clone the repository:
```bash
git clone <repository-url>
cd event-landing-page
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Configure environment variables:
   - Rename `.env.example` to `.env`
   - Add your Gmail credentials
   - Add your Google Maps API key in `templates/index.html`

4. Initialize the database:
```bash
python
>>> from app import db
>>> db.create_all()
>>> exit()
```

5. Run the application:
```bash
python app.py
```

The application will be available at `http://localhost:5000`

## Configuration

### Email Setup
1. Enable 2-factor authentication in your Gmail account
2. Generate an App Password
3. Use these credentials in your `.env` file

### Google Maps Setup
1. Get an API key from Google Cloud Console
2. Enable Maps JavaScript API
3. Replace `YOUR_API_KEY` in `templates/index.html`

## Project Structure

```
event-landing-page/
├── static/
│   ├── css/
│   │   └── styles.css
│   └── js/
│       └── main.js
├── templates/
│   └── index.html
├── app.py
├── requirements.txt
└── README.md
```

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a new Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.
