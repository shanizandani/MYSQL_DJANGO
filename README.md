﻿# MYSQL_DJANGO

# Employee Management API

This is a Django REST API for managing employees and departments in a company.

## Requirements

- Python 3.x
- Django 3.x
- Django REST framework

## Installation

1. Clone the repository to your local machine:

```bash
git clone https://github.com/your_username/employee-management-api.git
```

2. Install the required Python packages using pip:

```bash
pip install -r requirements.txt
```

3. Run database migrations:

```bash
python manage.py migrate
```

4. Start the development server:

```bash
python manage.py runserver
```

The API will be accessible at `http://127.0.0.1:8000/`.

## API Endpoints

### Department API

- **GET** `/department/`: Get a list of all departments.
- **GET** `/department/{id}/`: Get details of a specific department.
- **POST** `/department/`: Add a new department.
- **PUT** `/department/{id}/`: Update an existing department.
- **DELETE** `/department/{id}/`: Delete a department.

### Employee API

- **GET** `/employee/`: Get a list of all employees.
- **GET** `/employee/{id}/`: Get details of a specific employee.
- **POST** `/employee/`: Add a new employee.
- **PUT** `/employee/{id}/`: Update an existing employee.
- **DELETE** `/employee/{id}/`: Delete an employee.

### File Upload API

- **POST** `/employee/savefile/`: Upload a file (photo) for an employee.

## Usage

You can interact with the API using HTTP requests (e.g., using curl or Postman) or by integrating it into your frontend application.

### Examples

1. Add a new department:

```
POST http://127.0.0.1:8000/department/
{
  "DepartmentName": "HR"
}
```

2. Get all employees:

```
GET http://127.0.0.1:8000/employee/
```

3. Upload a photo for an employee:

```
POST http://127.0.0.1:8000/employee/savefile/
[Attach the file using the 'file' key in the request]
```

## Contributions

Feel free to fork this repository and submit pull requests if you want to contribute to the project.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
