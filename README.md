# Find My College: Navigating College Options with Ease

This repository contains the code for a Django-based website designed to simplify the college selection process for students. The platform provides comprehensive details and comparison tools for 50 colleges.

## Features

- **Real Placement Stats:** Displayed for each college to assist in informed decision-making.
- **College Details:** Includes information such as address, intake, fees, and amenities. Data is scraped using Selenium.
- **Interactive Map:** Shows college locations and calculates distances from the student’s location using geolocation APIs.
- **Comparison Tool:** A Python module is included for detailed college information and comparative graphs.

## Releases

The website is currently live and accessible [here](https://eamcet-colleges.onrender.com/).

## Installation

To get a local copy up and running, follow these simple steps:

1. **Clone the repository:**
   ```
   git clone https://github.com/Arshad-Ali-1a/findMyCollege.git
   ```

2. **Navigate to the project directory:**
   ```sh
   cd findMyCollege
   ```

3. **Create and activate a virtual environment:**
   ```sh
   python -m venv env
   or
   pipenv shell
   ```

4. **Install the required packages:**
   ```
   pip install -r requirements.txt
   ```

5. **Run the migrations:**
   ```
   python manage.py migrate
   ```

6. **Start the development server:**
   ```sh
   python manage.py runserver
   ```

7. **Access the website:**
   Open your browser and go to `http://127.0.0.1:8000/`

<br/>
<br/>

### Python module for College Copmarision

A custom Python module provides detailed information and comparison graphs. To use the module, import it in your scripts:
```python
from colleges import *

for college in College.instances.values():
    print(college,college.name)

College.graph("highest_salary")
```

Checkout demo.ipynb for more examples.
