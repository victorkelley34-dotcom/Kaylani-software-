# Kaylani Software

A FastAPI-based service for data processing, user management, and AI services.

## Features

- 🔐 **User Management** - User registration, authentication, and profile management
- 📊 **Data Processing** - APIs for processing, storing, and retrieving data
- 🤖 **AI Services** - Integration with AI/ML models for predictions and analysis
- 🔌 **RESTful API** - Clean, well-documented API endpoints
- 🗄️ **PostgreSQL** - Robust database for data persistence
- 🧪 **Testing** - Comprehensive test suite with pytest
- 📚 **Documentation** - Auto-generated API docs with Swagger UI

## Tech Stack

- **Framework**: FastAPI
- **Language**: Python 3.9+
- **Database**: PostgreSQL
- **ORM**: SQLAlchemy
- **Authentication**: JWT
- **Testing**: pytest

## Quick Start

### Prerequisites
- Python 3.9+
- PostgreSQL 12+

### Installation

```bash
# Clone repository
git clone https://github.com/victorkelley34-dotcom/Kaylani-software-.git
cd Kaylani-software-

# Create virtual environment
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Configure environment
cp .env.example .env

# Run application
uvicorn app.main:app --reload
```

### Access API
- API: http://localhost:8000
- Swagger UI: http://localhost:8000/docs
- ReDoc: http://localhost:8000/redoc

## API Endpoints

### Authentication
- `POST /api/v1/auth/register` - Register new user
- `POST /api/v1/auth/login` - Login user

### Users
- `GET /api/v1/users/me` - Get current user profile
- `PUT /api/v1/users/me` - Update user profile
- `GET /api/v1/users/{user_id}` - Get user by ID

### Data Processing
- `POST /api/v1/data/process` - Process data
- `GET /api/v1/data` - List user data
- `GET /api/v1/data/{data_id}` - Get data by ID
- `PUT /api/v1/data/{data_id}` - Update data
- `DELETE /api/v1/data/{data_id}` - Delete data

### AI Services
- `POST /api/v1/ai/predict` - Make AI prediction
- `POST /api/v1/ai/analyze` - Analyze data with AI
- `GET /api/v1/ai/models` - List available models

## Testing

```bash
# Run all tests
pytest

# Run with coverage
pytest --cov=app

# Run specific test
pytest tests/test_auth.py -v
```

## Project Structure

```
Kaylani-software-/
├── app/
│   ├── api/v1/          # API endpoints
│   ├── models/          # Database models
│   ├── schemas/         # Pydantic schemas
│   ├── services/        # Business logic
│   ├── utils/           # Utilities
│   ├── middleware/      # Custom middleware
│   ├── main.py          # FastAPI app
│   ├── config.py        # Configuration
│   ├── database.py      # Database setup
│   └── dependencies.py  # Dependencies
├── tests/               # Test suite
├── requirements.txt     # Dependencies
├── .env.example         # Environment template
└── README.md           # This file
```

## Repository Information

- **Repository**: victorkelley34-dotcom/Kaylani-software-
- **Repository ID**: 1264103458
- **Language**: Python

## License

MIT License

## Contact

For support, contact the development team.
