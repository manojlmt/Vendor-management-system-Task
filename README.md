# Vendor Management System using Django and Django REST Framework

A Vendor Management System built with Django and Django REST Framework. This system handles vendor profiles, purchase order tracking, and vendor performance metrics calculation.

## Table of Contents

1. [Installation](#installation)
2. [Usage](#usage)
3. [Features](#features)
4. [Contributing](#contributing)
5. [License](#license)

## Installation

To run this project locally, follow these steps:

1. Clone the repository:

```bash
git clone https://github.com/manojlmt/Vendor-management-system-Task.git
```
2. Install dependencies:

pip install -r requirements.txt

Configure MySQL database:
Create a MySQL database for the project.
Update the database settings in settings.py file located in vendor_management_system directory:
' 
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'your_database_name',
        'USER': 'your_database_user',
        'PASSWORD': 'your_database_password',
        'HOST': 'localhost',
        'PORT': '3306',
    }
}
'

3. Apply migrations:

python manage.py makemigrations
python manage.py migrate

4. Run the development server:
    
python manage.py runserver


## API Endpoints

# Vendor Profile Management:

POST /api/vendors/: Create a new vendor.
GET /api/vendors/: List all vendors.
GET /api/vendors/{vendor_id}/: Retrieve a specific vendor's details.
PUT /api/vendors/{vendor_id}/: Update a vendor's details.
DELETE /api/vendors/{vendor_id}/: Delete a vendor.

# Purchase Order Tracking:

POST /api/purchase_orders/: Create a purchase order.
GET /api/purchase_orders/: List all purchase orders with an option to filter by vendor.
GET /api/purchase_orders/{po_id}/: Retrieve details of a specific purchase order.
PUT /api/purchase_orders/{po_id}/: Update a purchase order.
DELETE /api/purchase_orders/{po_id}/: Delete a purchase order.

# Vendor Performance Evaluation:

GET /api/vendors/{vendor_id}/performance: Retrieve a vendor's performance metrics.

## Features:

1. Vendor Profile Management
2. Purchase Order Tracking
3. Vendor Performance Evaluation


## Postman Collection 

''' https://api.postman.com/collections/34693558-900b7a73-fcc4-46ae-83c7-d75ad5b07629?access_key=PMAT-01HWZQVS600QXGZX75RB2HSADT'''

