# Laravel 9.0 Essential Practice
This is the repository for the LinkedIn Learning course Laravel 9.0 Essential Training. The full course is available from.

Laravel, the open-source PHP web framework, has become one of the most widely used ecosystems for building scalable apps at lightning-quick speed. 

Learn about MVC architecture, how the Laravel framework is structured, routes and controllers, Blade files, models, and best practices for interacting with a database. Get tips on using various components in Laravel as you build your own simple note-taking app. From user authentication and routing, to CRUD operations and database relations, find out why the latest version, Laravel 9.0, allows you to build web apps quickly and easily, no matter where you are on your coding journey.


## Installing
1. To use these exercise files, you must have the following installed:
	- Docker
    - WSL2 (if using Windows OS)
    Instructions for installing both the above are covered in the course.
2. Clone this repository into your local machine using the terminal (Mac), CMD (Windows), or a GUI tool like SourceTree.
3. Navigate into your project directory
    ```
    cd <your-project-name>
    ```
4. Install project dependencies using the following command:
    ```
    docker run --rm \
    -u "$(id -u):$(id -g)" \
    -v $(pwd):/var/www/html \
    -w /var/www/html \
    laravelsail/php81-composer:latest \
    composer install --ignore-platform-reqs
    ```
    When using the laravelsail/phpXX-composer image, you should use the same version of PHP that you plan to use for your application (74, 80, or 81).
5. Create the .env file from the example file
    ```
    cp .env.example .env
    ```
6. Open the .env file and change the database configuration to the following
    ```
    DB_CONNECTION=mysql
    DB_HOST=mysql
    DB_PORT=3306
    DB_DATABASE=<your-project-name>
    DB_USERNAME=sail
    DB_PASSWORD=password
    ```
7. Start Sail with the command
    ```
    sail up
    ```
    Leave this command running.
8. Open a new terminal tab to generate application key
    ```
    sail artisan key:generate
    ```
9. Migrate database tables
    ```
    sail artisan migrate
    ```
10. Go to localhost on your browser to view the application



### Certified
Jahid Al Mamun
rjs.jahid22@gmail.com

![Laravel Certification of Jahid Al Mamun](https://www.linkedin.com/learning/certificates/037aef9ec21a4b692cad0df8677e4f500a301bcfdc40678f47cd3bb8b04d227f)
