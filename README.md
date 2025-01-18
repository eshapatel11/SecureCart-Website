# SecureCart: A Secure E-Commerce Platform 🛒🔒

Welcome to SecureCart, an e-commerce platform designed with a strong emphasis on security, scalability, and user experience. Developed using the Django framework, SecureCart integrates robust features to provide a seamless and secure shopping experience.

---

## Key Features 🌟

### **Authentication & Authorisation**
- **Secure Login & Registration**: Passwords are securely hashed using PBKDF2.
- **Role-Based Access Control (RBAC)**: Access restricted based on user roles (Customer/Admin).
- **Session Management**: Ensures secure and consistent user sessions.

### **Customer Features**
- Browse and search for products.
- Add items to the cart and proceed to checkout.
- Manage personal profiles and view/download order invoices.
- **Secure Payment Workflow**: Protects sensitive information during checkout.

### **Admin Features**
- Add, update and delete products via a feature-rich admin dashboard.
- Manage orders, including viewing, updating statuses.
- View and manage customer details.

### **Security**
- **CSRF Protection**: Prevents cross-site request forgery.
- **Data Encryption**: HTTPS for secure data transmission; AES-256 for sensitive data at rest.
- **Input Validation**: Validates user inputs to prevent SQL injection and XSS attacks.
- **Audit Logging**: Logs login attempts and admin actions for compliance.

---

## Technologies Used 🛠️
- **Backend**: Python, Django Framework
- **Frontend**: HTML, CSS (Bootstrap), JavaScript (AJAX for dynamic updates)
- **Database**: SQLite
- **PDF Generation**: `xhtml2pdf` for invoices
- **Security**: Django Middleware, HTTPS, AES-256 encryption

---

## Getting Started 🚀

### **Prerequisites**
Ensure the following are installed on your system:
- Python (>= 3.8)
- Django (>= 4.0)
- Virtualenv (optional but recommended)

### **Setup Instructions**
1. Clone the repository:
    ```bash
    git clone https://github.com/eshapatel11/SecureCart-Website.git
    cd SecureCart-Website
    cd ecommerce-master
    ```

2. Create and activate a virtual environment:
    ```bash
    python -m venv env
    source env/bin/activate  # On Windows: env\Scripts\activate
    ```

3. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Apply migrations to set up the database:
    ```bash
    python manage.py migrate
    ```

5. Run the development server:
    ```bash
    python manage.py runserver
    ```

6. Open your browser and visit:
    ```
    http://127.0.0.1:8000/
    ```


---

## Directory Structure 📂
```plaintext
SecureCart/
├── ecom/                  # Main app containing core logic
│   ├── templates/         # HTML templates for the frontend
│   ├── static/            # Static files (CSS, JS, images)
│   ├── models.py          # Database models
│   ├── views.py           # Business logic
│   ├── urls.py            # URL routing
│   └── forms.py           # Form validation logic
├── manage.py              # Django entry point
├── db.sqlite3             # SQLite database file
├── requirements.txt       # Python dependencies
└── README.md              # Project README file
