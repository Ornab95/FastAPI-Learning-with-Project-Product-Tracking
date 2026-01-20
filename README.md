# AB Trac - Product Management System

A modern full-stack product inventory management application built with FastAPI and React.

## Features

- ✅ Create, read, update, and delete products
- ✅ Search and filter products
- ✅ Sortable product table
- ✅ Responsive modern UI
- ✅ Real-time data updates
- ✅ Database persistence with SQLAlchemy

## Tech Stack

**Backend:**
- FastAPI (Python web framework)
- SQLAlchemy (Database ORM)
- Pydantic (Data validation)
- SQLite (Database)

**Frontend:**
- React 18
- Axios (HTTP client)
- Modern CSS with responsive design

## Installation

### Prerequisites
- Python 3.8+
- Node.js 16+
- npm or yarn

### Backend Setup

1. Clone the repository:
```bash
git clone https://github.com/Ornab95/FastAPI-Learning-with-Project-Product-Tracking.git
cd FastAPI-Learning-with-Project-Product-Tracking
```

2. Install Python dependencies:
```bash
pip install -r requirements.txt
```

3. Start the FastAPI server:
```bash
uvicorn main:app --reload
```

The API will be available at `http://localhost:8000`

### Frontend Setup

1. Navigate to the frontend directory:
```bash
cd frontend
```

2. Install dependencies:
```bash
npm install
```

3. Start the React development server:
```bash
npm start
```

The frontend will be available at `http://localhost:3000`

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/products` | Get all products |
| GET | `/products/{id}` | Get product by ID |
| POST | `/products` | Create new product |
| PUT | `/products/{id}` | Update product |
| DELETE | `/products/{id}` | Delete product |

## Product Schema

```json
{
  "id": 1,
  "name": "Product Name",
  "description": "Product description",
  "price": 99.99,
  "category": "Category Name"
}
```

## Usage

1. Start both backend and frontend servers
2. Open `http://localhost:3000` in your browser
3. Use the form to add new products
4. View, edit, or delete products in the table
5. Use the search bar to filter products

## Project Structure

```
FactAPI/
├── main.py                 # FastAPI application
├── requirements.txt        # Python dependencies
├── model/
│   ├── product_model.py   # Pydantic models
│   └── user.py
├── database.py            # Database configuration
├── database_model.py      # SQLAlchemy models
└── frontend/
    ├── src/
    │   ├── App.js         # Main React component
    │   ├── App_clean.css  # Styling
    │   └── index.js       # React entry point
    ├── public/
    └── package.json       # Node.js dependencies
```

## Development

### Adding New Features

1. **Backend**: Add new endpoints in `main.py`
2. **Frontend**: Update `App.js` for UI changes
3. **Database**: Modify models in `database_model.py`

### API Documentation

FastAPI automatically generates interactive API documentation:
- Swagger UI: `http://localhost:8000/docs`
- ReDoc: `http://localhost:8000/redoc`

## License

This project is open source and available under the MIT License.
