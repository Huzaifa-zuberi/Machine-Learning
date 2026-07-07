# Machine Learning

Machine learning projects and experiments.

## Projects

### PulseDB — Music Streaming Platform

Full-stack database project: SQL Server backend + Python Flask API + browser dashboard.

\Machine-Learning/
├── backend/
│   ├── app.py              # Flask REST API (6 endpoints)
│   └── requirements.txt    # Python dependencies
├── database/
│   └── project.sql         # SQL Server schema, data, queries & views
└── frontend/
    └── index.html          # Single-page dashboard
\
### Setup

**1. Database** — Run \database/project.sql\ in SQL Server Management Studio.

**2. Backend API**
\\ash
cd backend
pip install -r requirements.txt
python app.py
\API starts at \http://localhost:5000\.

**3. Frontend** — Open \rontend/index.html\ in a browser.

### API Endpoints

| Method | Path | Description |
|--------|------|-------------|
| GET | \/api/songs\ | All songs with artist & genre |
| GET | \/api/trending\ | Top 5 most-streamed songs |
| GET | \/api/fans\ | Users with 3+ streams |
| GET | \/api/users\ | User list for dropdown |
| GET | \/api/songs/list\ | Song list for dropdown |
| POST | \/api/stream\ | Record a new stream |
