# Car Listings Collector

This project is a web application that scrapes car listing websites to find and display the best deals for specific car models. Built with a FastAPI backend and a modern frontend (to be developed), this app demonstrates scraping, data processing, and visualization techniques in a clean and structured codebase.

---

## Table of Contents

1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Tech Stack](#tech-stack)
4. [Folder Structure](#folder-structure)
5. [Setup Instructions](#setup-instructions)
    - [Prerequisites](#prerequisites)
    - [Backend Setup](#backend-setup)
6. [Usage](#usage)
7. [Development Roadmap](#development-roadmap)
8. [Contributing](#contributing)
9. [License](#license)

---

## Project Overview

**The Car Listings Collector** helps users save time and money by automating the search for affordable car deals, reducing the hassle of manual browsing across multiple platforms.

Key objectives of this project:
- Automate web scraping tasks using modern Python tools.
- Develop a scalable API to serve processed car listing data.
- Build a user-friendly frontend for filtering and visualization.

---

## Features

1. **Web Scraping**:
   - Scrapes car listings from popular websites.
   - Filters and sorts listings based on price, model, and location.

2. **Backend API**:
   - FastAPI-powered API for serving scraped data.
   - Endpoints for listing retrieval, filtering, and updates.

3. **Frontend (To Be Developed)**:
   - Interactive UI for browsing and filtering car listings.
   - Visualization tools for comparing prices and trends.

4. **Data Processing**:
   - Cleans and normalizes data for consistency.
   - Supports geolocation-based proximity searches.

---

## Tech Stack

| **Component**   | **Technology**    | **Purpose**                                      |
|------------------|-------------------|--------------------------------------------------|
| **Backend**      | FastAPI           | REST API for data access and management          |
| **Frontend**     | (Planned) Svelte | Responsive and modern user interface             |
| **Database**     | SQLite (Planned) | Lightweight and simple storage for listings      |
| **Web Scraping** | Playwright        | Collects listing data from multiple websites     |
| **Task Scheduler** | (Planned) Celery | Automates periodic scraping tasks                |
| **Containerization** | Docker         | Packages the app for consistent development and deployment |

---

## Folder Structure

```
car-listings-collector/
├── backend/
│   ├── app/
│   │   └── main.py          # FastAPI entry point
│   ├── venv/                # Virtual environment
│   ├── requirements.txt     # Backend dependencies
│   └── __pycache__/         # Autogenerated files
├── frontend/                # (To Be Developed)
├── data/                    # Directory for temporary scraped data
├── README.md                # Project documentation
└── .gitignore               # Git ignored files and folders
```

## Setup Instructions

### Prerequisites

Ensure the following tools are installed on your system:
    - Python 3.13+ 
    - Git
    - Node.js (Optional) for frontend development

### Backend Setup

1. Clone the repository:

bash
git clone https://github.com/RPetrela-Dev/car-listings-collector.git
cd car-listings-collector/backend


2. Setup the virtual environment:

bash
python -m venv venv
source venv/Scripts/activate  # For Windows


3. Install dependencies:

bash
pip install -r requirements.txt


4. Run the FastAPI server:

bash
uvicorn app.main:app --reload


## Usage

1. Access the API:
    - Open your browser and visit http://127.0.0.1:8000.
    - API documentation is available at http://127.0.0.1:8000/docs.

2. (Planned) Frontend:
    - Once developed, navigate to the frontend URL to browse car listings.

## Development Roadmap

1. **Phase 1**: Backend Setup
    - FastAPI API and basic scraping scripts.

2. **Phase 2**: Advanced Scraping and Task Automation
    - Use Playwright for dynamic web scraping.
    - Schedule scraping tasks using Celery.

3. **Phase 3**: Frontend Development
    - Build a modern UI with Svelte or React.
    - Integrate frontend with the backend API.

4. **Phase 4**: Deployment
    - Package the app with Docker for deployment.

## Contributing

Contributions are welcome! To contribute:

1. Fork this repository.
2. Create a new branch: git checkout -b feature-name.
3. Make your changes and commit them: git commit -m 'Add feature-name'.
4. Push to the branch: git push origin feature-name.
5. Submit a pull request.

## Credits

If you use this code or any part of it in your own projects, please provide credit to the original author. You can credit by:

- Mentioning the project and linking back to this repository in your documentation.
- Acknowledging [Rey Petrela](https://github.com/RPetrela-Dev) in your work.

## License

This project is licensed under the MIT License. See the LICENSE file for details.