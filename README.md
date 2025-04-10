# Security+ Exam Preparation Website

A modern, feature-rich web application for practicing Security+ exam questions with a beautiful dark theme UI.

## Features

- User authentication and progress tracking
- Customizable practice exams
- Multiple timer options (per question or total exam time)
- Instant feedback on answers with explanations
- Progress tracking and exam history
- Modern dark theme UI with animations
- PDF question import functionality

## Setup Instructions

1. Create a virtual environment and activate it:
```bash
python -m venv venv
.\venv\Scripts\activate
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Import questions from your PDF:
```bash
python pdf_import.py path/to/your/questions.pdf [options]
```

PDF Import Options:
- `--verbose` or `-v`: Enable verbose output for debugging
- `--skip-duplicates`: Skip questions that already exist in the database
- `--batch-size N`: Set database batch size (default: 50)
- `--dry-run`: Extract questions without inserting into database

4. Run the application:
```bash
python app.py
```

5. Visit http://localhost:5000 in your browser

## Features

### Exam Configuration
- Choose number of questions (20, 50, 90, or 180)
- Timed or practice mode
- Per-question timer (1 minute each) or total exam time
- Track progress with question navigation

### User Features
- Create an account to track progress
- View exam history and statistics
- Resume interrupted exams
- Review incorrect answers

### UI Features
- Modern dark theme
- Responsive design
- Animated transitions
- Progress tracking
- Interactive question navigation

## Technologies Used

- Flask (Python web framework)
- SQLAlchemy (Database ORM)
- TailwindCSS (Styling)
- Alpine.js (JavaScript framework)
- PyPDF2 (PDF parsing)
- Font Awesome (Icons)
