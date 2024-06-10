Flask Exercise Documentation
This project is a Flask application developed as an exercise to analyze office, employee, product, and customer data from a provided database. Below is the documentation for setting up and running the application.

Setup Instructions
Clone the Repository:

bash
Copiar código
git clone <repository_url>
cd <repository_name>
Install Dependencies:

bash
Copiar código
pip install -r requirements.txt
Set Environment Variables:
Create a .env file in the root directory and add the following variables:

env
Copiar código
DB_USER=root
DB_PASSWORD=root123
DB_HOSTNAME=localhost
DB_NAME=classicmodels
SQLALCHEMY_TRACK_MODIFICATIONS=False
Database Setup:

Ensure MySQL is installed and running.
The provided MySQL sample database file mysqlsampledatabase.sql will be imported automatically during application startup.
Run the Application:

bash
Copiar código
python3 app.py
The application will be accessible at http://localhost:5000/.

Project Structure
app.py: Flask application entry point containing route definitions.
models.py: Database models using SQLAlchemy ORM.
templates/: HTML templates for rendering pages.
static/: Static files (CSS, JS, images).
Functionality Overview
Offices: Analyze office details including employee count and number of customers.
Products: View low stock products and best-selling products.
Employees: Insights into employee data including sales volume and purchase frequency.
Customers: Identify top 20% customers by total spent for potential discounts.
Additional Notes
The application is designed to run on Ubuntu, adjustments may be needed for other platforms.
Docker configuration is provided in docker-compose.yml for containerized deployment.
Code follows PEP8 guidelines and includes documentation for improved readability.
