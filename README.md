# Scholarship Recommendation System

## Overview
The Scholarship Recommendation System is a data-driven web application designed to help users discover scholarships based on their eligibility criteria. The system filters scholarship opportunities using user inputs such as **age, gender, and social category**, providing personalized recommendations efficiently.

The project combines **data processing, backend API development, and frontend integration** to create an interactive recommendation platform.

---

## Features

- Personalized scholarship filtering based on:
  - Age
  - Gender
  - Social Category

- RESTful API implementation using Flask

- Dynamic frontend interaction using JavaScript

- Real-time scholarship search functionality

- Pagination support for handling large datasets efficiently

- JSON-based API responses for seamless frontend-backend communication

- Interactive and user-friendly interface

---

## Tech Stack

### Backend
- Python
- Flask
- Pandas

### Frontend
- HTML
- CSS
- JavaScript

### Data Processing
- Pandas
- CSV Dataset Handling

### API Development
- RESTful API Architecture

---

## Project Architecture

```
Scholarship Recommendation System
│
├── app.py                     # Flask backend server
├── templates/
│   └── index.html            # Frontend UI
├── static/
│   ├── script.js             # Search & pagination logic
│   └── styles.css            # Styling
├── data/
│   └── recommendation_dataset.csv
└── README.md
```

---

## Workflow

1. User enters eligibility details:
   - Age
   - Gender
   - Social Category

2. Frontend sends query parameters to Flask API.

3. Backend processes filters using Pandas.

4. Matching scholarships are retrieved from the dataset.

5. Results are returned in JSON format.

6. Frontend dynamically renders scholarship recommendations with pagination.

---

## Data Science Perspective

This project incorporates multiple data science concepts:

- Data preprocessing and cleaning
- Feature-based filtering
- Structured dataset analysis
- Query optimization
- Recommendation logic development
- Data-driven decision systems

---

## API Endpoint

### Search Scholarships

```http
GET /search
```

### Query Parameters

| Parameter | Type | Description |
|------------|-------|-------------|
| age | Integer | User age |
| gender | String | User gender |
| social_category | String | Social category |
| page | Integer | Pagination page number |

Example:

```bash
/search?age=18&gender=Female&social_category=SC&page=1
```

Response:

```json
[
  {
    "scheme_name": "Scholarship A",
    "description": "Scholarship details",
    "gender": "Female",
    "social_category": "SC",
    "age": 18
  }
]
```

---

## Installation

Clone the repository:

```bash
git clone <repository-url>
```

Navigate to the project folder:

```bash
cd Scholarship-Recommendation-System
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the application:

```bash
python app.py
```

Open browser:

```
http://127.0.0.1:5000
```

---

## Future Improvements

- User authentication and authorization
- Database integration (PostgreSQL/MySQL)
- Machine learning-based recommendation engine
- User profile personalization
- Bookmark and save scholarship options
- Deployment using Docker and cloud services

---

## Key Learnings

- REST API development with Flask
- Data filtering and preprocessing using Pandas
- Frontend-backend integration
- Pagination implementation
- Building scalable recommendation systems

---

## Author

**Diptanil Paul**

Data Science | Machine Learning | Full Stack Development
