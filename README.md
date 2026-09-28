# 💰 Finance — Full-Stack Web Application

A full-stack personal finance and stock-trading web application built with **Python, Flask, SQL, HTML, CSS, and JavaScript**.

The application allows users to create accounts, view stock information, buy and sell shares, track their portfolio, and review transaction history through a web-based interface.

## 🚀 Features

* 🔐 User registration and authentication
* 💵 Portfolio and cash balance management
* 📈 Stock price lookup
* 🛒 Buy and sell stocks
* 📊 Portfolio tracking
* 🧾 Transaction history
* 🗄️ SQL-based data persistence
* 🎨 Responsive web interface
* ⚠️ Error handling and validation
* 🧪 Automated application tests

## 🛠️ Tech Stack

### Backend

* Python
* Flask
* Flask-SQLAlchemy
* SQL
* Jinja2

### Frontend

* HTML5
* CSS3
* JavaScript
* Jinja templates
* SVG-based illustrations

### Development & Testing

* Pipenv
* Pytest
* GitHub Actions
* Docker-compatible project structure

## 🏗️ Project Structure

```text
finance-full-stack-web-app/
│
├── application.py          # Flask application
├── helpers.py              # Helper functions
├── Pipfile                # Python dependencies
├── Pipfile.lock
├── README.md
│
├── templates/              # HTML/Jinja templates
│   ├── layout.html
│   ├── index.html
│   ├── landing.html
│   ├── login.html
│   ├── register.html
│   ├── buy.html
│   ├── sell.html
│   ├── bought.html
│   ├── sold.html
│   ├── history.html
│   └── ...
│
├── static/
│   ├── styles.css
│   ├── index.js
│   ├── images/
│   └── favicon/
│
├── tests/
│   ├── test_app.py
│   └── test_views.py
│
└── .github/
    └── workflows/
```

## ⚙️ Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/adityaasinghhh/finance-full-stack-web-app.git
cd finance-full-stack-web-app
```

### 2. Install Python dependencies

Make sure Python and pip are installed.

Using Pipenv:

```bash
pip install pipenv
pipenv install
```

Activate the virtual environment:

```bash
pipenv shell
```

### 3. Configure the API key

The application uses a stock-market API to retrieve stock information.

Create a `.env` file in the project root:

```env
API_KEY=your_api_key_here
```

**Never commit your `.env` file or API credentials to GitHub.**

### 4. Initialize the database

The application uses SQLAlchemy for database interaction.

Start Python:

```bash
python
```

Then:

```python
from application import db
db.create_all()
```

Exit Python:

```python
exit()
```

### 5. Run the application

```bash
python application.py
```

The application will start locally and can be accessed through the URL shown by Flask.

Alternatively:

```bash
flask run
```

## 🗄️ Database Design

The application maintains information related to users, portfolios, purchases, and sales.

Conceptually, the database contains:

```text
Users
  │
  ├── Portfolio
  │
  ├── Bought Transactions
  │
  └── Sold Transactions
```

This allows the application to maintain each user's holdings and transaction history independently.

## 🧪 Testing

The project includes automated tests for application behavior and views.

Run the test suite with:

```bash
pytest
```

## 🔐 Security Considerations

The application includes authentication and server-side validation for financial transactions.

For local development:

* Store API keys in environment variables.
* Never commit `.env` files.
* Use strong passwords when testing authentication.
* Use a production-grade database and secret-management solution before deploying publicly.

## 📚 What I Learned

This project provided hands-on experience with:

* Building a full-stack application using Flask
* Designing and interacting with SQL databases
* Implementing authentication and sessions
* Creating REST-style application routes
* Connecting a backend to external APIs
* Building dynamic pages with Jinja2
* Handling financial transaction workflows
* Writing automated tests
* Structuring a maintainable web application

## 🔮 Future Improvements

Potential improvements include:

* Modern authentication with OAuth/JWT
* Improved portfolio analytics and visualizations
* Real-time stock-price updates
* More advanced transaction reporting
* REST API documentation
* PostgreSQL support for production deployment
* Docker-based deployment
* Improved responsive UI
* Role-based access control
* Comprehensive API and integration tests

## 👨‍💻 Author

**Aditya Singh**

Computer Science Engineering

GitHub: [@adityaasinghhh](https://github.com/adityaasinghhh)

---

## 📌 Disclaimer

This project is intended for **educational and demonstration purposes**. Stock information and financial functionality should not be considered financial advice.
