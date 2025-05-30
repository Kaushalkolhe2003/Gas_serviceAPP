
# Gas Utility Service Application

This Django-based application is designed for gas utility companies, providing a platform where customers can submit service requests, track their status, and manage their account information. Customer service representatives (CSR) are equipped with tools to manage customer requests effectively.

## Features

**Customer Portal**:
- Submit service requests.
- Track the status of service requests.
- View and update account information.

**CSR Portal**:
- Manage customer service requests.
- Provide support and assistance to customers.

## Project Structure

- **Frontend**: Utilizes [UIKit](https://getuikit.com) for UI components.
- **Backend**: Built with the Django web framework, powered by a MySQL database.

## Technologies Used

- **Programming Language**: Python (3.11)
- **Web Framework**: Django (>= 4.1)
- **Database**: MySQL (Port: 3306)
- **UI Framework**: UIKit

## Setup Instructions

### Clone the repository:

```bash
git clone https://github.com/your-username/gas-utility-app.git
cd gas-utility-app
```

### Install the dependencies:

Ensure Python 3.11 is installed. Install the required dependencies:

```bash
pip install -r requirements.txt
```

### Configure MySQL:

Make sure MySQL is running on port `3306` (default MySQL port). You can configure it in the Django `settings.py` file:

```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'your_db_name',
        'USER': 'your_db_user',
        'PASSWORD': 'your_db_password',
        'HOST': 'localhost',
        'PORT': '3306',
    }
}
```

### Set up the database and apply migrations:

```bash
python manage.py makemigrations
python manage.py migrate
```

### Run the development server:

```bash
python manage.py runserver
```

Open a browser and go to `http://127.0.0.1:8000/` to view the application.

## Key URLs

- **Home Page**: `/`
- **Customer Login**: `/login/`
- **Customer Account Information**: `/customer/account_information/`
- **Submit a Service Request**: `/customer/service_request/`
- **Request Status**: `/customer/sr_details/`
- **CSR Tool**: `/csr/sr_tool/`

## How to Contribute

Contributions are welcome! Follow the steps below to contribute:

1. Fork the repository.
2. Create a new branch for your feature or fix:

    ```bash
    git checkout -b feature-branch
    ```

3. Commit your changes:

    ```bash
    git commit -m "Description of changes"
    ```

4. Push the branch to your fork:

    ```bash
    git push origin feature-branch
    ```

5. Open a Pull Request describing your changes.

## Troubleshooting

- **Database Issues**: Ensure MySQL is running on port `3306`. Verify the database configuration in `settings.py` matches your MySQL instance.
- **UI Problems**: Ensure UIKit is correctly linked in the base templates.

## Contact

If you encounter any issues, feel free to reach out:

- **Name**: Kaushal Kolhe
- **Email**: kolhekaushal2003@gmail.com
- **Phone**: +91 7887458667
