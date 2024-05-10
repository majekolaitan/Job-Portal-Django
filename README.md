## TechConnect - Job Posting Platform

TechConnect is a powerful job posting platform developed using Django, a Python web framework. It provides a seamless experience for both employers and job seekers, facilitating the recruitment process effectively.

### Setup Instructions

#### Using Docker

Follow these steps to set up and run the TechConnect application using Docker:

##### Prerequisites

- Docker installed on your system ([Install Docker](https://docs.docker.com/get-docker/))

##### Clone the Repository

```bash
git clone <repository-url>
cd <repository-directory>
```

##### Build the Docker Image

```bash
docker build -t techconnect .
```

##### Run the Docker Container

```bash
docker run -p 8000:8000 techconnect
```

#### Accessing the Application

Once the Docker container is running, you can access the TechConnect application by visiting [http://localhost:8000](http://localhost:8000) in your web browser.

#### Creating a Superuser (Optional)

To administer the application at the `/admin` route, create a superuser with the following command:

```bash
docker exec -it <container-id> python manage.py createsuperuser
```

Replace `<container-id>` with the ID of your Docker container.

### Usage

- **Employer**:

  - Register your company and log in.
  - Post job listings.
  - Manage job postings from the dashboard.

- **Employee**:
  - Create an account or log in.
  - Browse job listings.
  - Bookmark interesting jobs.
  - Apply for positions.

### Administration

#### User Administration

- User Management
- Password Management
- User Permissions
- Forms for User Creation and Update

#### Job Administration

- Admins can manage categories related to jobs.
- Admins can view a list of applicants for jobs.
- Each applicant is listed with the job they applied for, the user who applied, and the timestamp of the application.
- Admins can view and manage job postings.
- Each job is listed with its title, publication status, closure status, and timestamp.
- Admins can manage bookmarked jobs.
- Each bookmarked job is listed with the job itself, the user who bookmarked it, and the timestamp of bookmarking.

### Project Structure

- **`/account`**: Handles user authentication and management.
- **`/job`**: Manages job postings and applications.
- **`/jobapp`**: Additional features related to job applications and management.
- **`/static`**: Contains static files like CSS, JavaScript, and images.
- **`/template`**: HTML templates for different sections of the website.
- **`Dockerfile`**: Docker configuration file.
- **`requirements.txt`**: List of Python dependencies.
- **`manage.py`**: Django management script.

### Setup Without Docker

If you prefer not to use Docker, follow these steps to set up the TechConnect application directly:

#### Prerequisites

- Python 3 installed on your system ([Install Python 3](https://www.python.org/downloads/))
- pip package manager

#### Clone the Repository

```bash
git clone <repository-url>
cd <repository-directory>
```

#### Install Python Dependencies

```bash
pip install -r requirements.txt
```

#### Apply Database Migrations

```bash
python manage.py makemigrations
python manage.py migrate
```

#### Collects all static files in your apps

```bash
python manage.py collectstatic
```

#### Create a Superuser (Optional)

```bash
python manage.py createsuperuser
```

#### Run the Django Development Server

```bash
python manage.py runserver
```

#### Accessing the Application

Once the server is running, you can access the TechConnect application by visiting [http://localhost:8000](http://localhost:8000) in your web browser.

#### Accessing the Admin Panel

You can access the Django admin panel by visiting [http://localhost:8000/admin](http://localhost:8000/admin) in your web browser. Here, you can perform user and job administration tasks as described above.

### Support

If you encounter any issues or have any questions, feel free to [create an issue](<repository-url>/issues) in the repository.

### Contributing

Contributions are welcome! Fork the repository, make your changes, and submit a pull request.

### License

This project is licensed under the [MIT License](LICENSE).

### Acknowledgements

Special thanks to the Django community for their amazing work on the framework.

### Author

Olaitan Majekodunmi - [Your Website or GitHub Profile]

![Settings Window](https://raw.github.com/majekolaitan/Django-Job-Portal/master/screenshots/screencapture-127-0-0-1-8000-2020-05-08-17_03_46.png)

![Settings Window](https://raw.github.com/majekolaitan/Django-Job-Portal/master/screenshots/screencapture-127-0-0-1-8000-jobs-2020-05-08-17_40_01.png)

![Settings Window](https://raw.github.com/majekolaitan/Django-Job-Portal/master/screenshots/screencapture-127-0-0-1-8000-job-79-2020-05-08-16_59_55.png)

![Settings Window](https://raw.github.com/majekolaitan/Django-Job-Portal/master/screenshots/screencapture-127-0-0-1-8000-job-create-2020-05-08-17_00_46.png)

![Settings Window](https://raw.github.com/majekolaitan/Django-Job-Portal/master/screenshots/screencapture-127-0-0-1-8000-dashboard-2020-05-08-17_01_07.png)

![Settings Window](https://raw.github.com/majekolaitan/Django-Job-Portal/master/screenshots/screencapture-127-0-0-1-8000-dashboard-employer-job-54-applicants-2020-05-08-17_01_34.png)

<div align="center">
    <h3>========Thank You=========</h3>
</div>
