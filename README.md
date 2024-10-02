# Crick Informer

**Crick Informer** is a web application built using Spring Boot (backend) and Angular (frontend). This application provides real-time cricket information by scraping data from various cricket websites.

## Table of Contents
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Setup and Installation](#setup-and-installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)
- [License](#license)

## Features
- Live cricket scores and updates.
- Player statistics and team details.
- Upcoming matches and schedules.
- Web scraping from popular cricket websites for real-time data.
  
## Technologies Used
### Backend:
- **Spring Boot** - RESTful API backend.
- **Java 17** - Programming language.
- **Jsoup** - For scraping cricket data from websites.
- **MySQL** - Database for storing scraped data.
  
### Frontend:
- **Angular** - Single-page application framework.

### Other:
- **Maven** - Dependency management.
- **Node.js & NPM** - For managing Angular dependencies and building the frontend.

## Setup and Installation

### Prerequisites:
- Java 17
- Maven
- Node.js and NPM
- MySQL
  
### Backend (Spring Boot):
1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/crick-informer.git
    cd crick-informer/backend
    ```
2. Configure the database connection in `application.properties`:
    ```properties
    spring.datasource.url=jdbc:mysql://localhost:3306/crickinfo(db name)
    spring.datasource.username=root
    spring.datasource.password=yourpassword
    ```
3. Build the project using Maven:
    ```bash
    mvn clean install
    ```
4. Run the Spring Boot application:
    ```bash
    mvn spring-boot:run
    ```

### Frontend (Angular):
1. Navigate to the frontend directory:
    ```bash
    cd ../frontend
    ```
2. Install dependencies:
    ```bash
    npm install
    ```
3. Run the Angular development server:
    ```bash
    ng serve
    ```
4. Open your browser and go to `http://localhost:4200`.

## Usage
Once the application is up and running, you can browse live cricket updates, view player and team statistics, and explore upcoming matches.

### Web Scraping
Data is scraped from cricket websites in real time using the `Jsoup` library in Spring Boot. Ensure the websites are accessible and that scraping complies with their terms of service.


## Contributing
Feel free to contribute to the project by submitting a pull request or reporting issues. Please ensure that you follow the project's coding standards and guidelines.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
