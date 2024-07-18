# Estate App

Estate App is a real estate web application built with Django that allows users to search for properties, book appointments for property viewings, and interact with real estate agents. Administrators can manage properties through the admin site.

## Features

- **User Features**
  - View available properties
  - Filter properties by price
  - Book appointments for property viewings
  - Real-time chat with agents

- **Admin Features**
  - Add, update, and delete properties
  - Manage user appointments

## Requirements

The following Python packages are required to run the project:

aiomysql==0.2.0
asgiref==3.6.0
certifi==2022.12.7
charset-normalizer==3.2.0
distlib==0.3.6
Django==4.2.1
django-filter==23.3
et-xmlfile==1.1.0
filelock==3.12.0
idna==3.4
openpyxl==3.1.2
pika==1.3.1
Pillow==9.5.0
pipenv==2023.4.29
platformdirs==3.5.0
PyMySQL==1.1.0
requests==2.31.0
sqlparse==0.4.4
tzdata==2023.3
urllib3==2.0.4
virtualenv==20.23.0
virtualenv-clone==0.5.7
mysqlclient==2.1.1


## Environment Variables

Set the following environment variables to configure the database connection:

REALESTATE_DB=<your-database-name>
database_username=<your-database-username>
database_password=<your-database-password>


## Setup Instructions

1. **Clone the repository:**

    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

2. **Install dependencies:**

    Using pipenv:

    ```bash
    pipenv install
    ```

    Using pip:

    ```bash
    pip install -r requirements.txt
    ```

3. **Set up the database:**

    Ensure you have MySQL installed and create a database for the project. Set the environment variables as mentioned above.

4. **Run migrations:**

    ```bash
    python manage.py migrate
    ```

5. **Create a superuser:**

    ```bash
    python manage.py createsuperuser
    ```

    Follow the prompts to create a superuser account.

6. **Run the development server:**

    ```bash
    python manage.py runserver
    ```

    The application will be accessible at `http://127.0.0.1:8000/`.

## Usage

- Access the admin site at `http://127.0.0.1:8000/admin` and log in using the superuser credentials.
- From the admin site, add, update, or delete properties.
- Visit the main site to view, filter, and book appointments for properties.

## Contribution

Feel free to open issues or submit pull requests for any improvements or bug fixes.

## License

This project is licensed under the MIT License.

