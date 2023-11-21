# Job Application Project

## Description
This project is a job application management system built with Symfony and MySQL. It allows users to submit job applications and search for existing applications. The application form includes fields such as name, surname, email, telephone number, expected salary, position, and level. 

## Features
- **Submit Job Applications**: Users can submit job applications by filling out a form with their personal details and job preferences.
- **Search Applications**: Users can search for existing applications using four modes: ID, new, old, and all.

## Endpoints
The application has the following endpoints:
1. `job_application_add`: For adding a new job application.
2. `job_application_show`: For showing a specific job application by ID.
3. `job_application_old`: For showing old job applications.
4. `job_application_new`: For showing new job applications.
5. `job_application_all`: For showing all job applications.

## Installation
1. Clone the repository to your local machine.
2. Install Symfony and MySQL if not already installed.
3. Run `Set-ExecutionPolicy RemoteSigned -Scope CurrentUser` and then `irm get.scoop.sh | iex` to install Scoop
4. Run `scoop install symfony-cli` to install Symfony CLI
5. Run `composer install` to install the necessary dependencies.
6. Run `composer require symfony/runtime` to install symfony/runtime
7. Configure your MySQL database in the `.env` file.
8. Run `php bin/console doctrine:database:create` to create the database.
9. Run `php bin/console doctrine:migrations:migrate` to create the necessary tables.
10. Start the Symfony server using `symfony server:start`.
11. Open your web browser and navigate to http://127.0.0.1:8000 to access the application.

## Database Configuration
The project uses a MySQL database. The database configuration is located in the `.env` file. You will need to provide the database host, port, user, password, and database name.

## Form Fields
The job application form includes the following fields:
- `First name`: The applicant's first name.
- `Second name`: The applicant's second name (Optional).
- `Surname`: The applicant's last name.
- `Date of birth`: The applicant's date of birth (Optional).
- `Email`: The applicant's email address.
- `Telephone Number`: The applicant's contact number.
- `Expected Salary`: The salary that the applicant expects to receive.
- `Position`: The job position that the applicant is applying for.
- `Level`: The applicant's level of expertise or experience (The level depends on salary).

## Usage
After installation, you can start submitting job applications and searching for existing applications. Enjoy using the application and feel free to contribute!

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change. Please make sure to update tests as appropriate.

