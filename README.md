## Dockerized PHP Repository

### Overview

This repository contains a Dockerized PHP environment for seamless development and deployment.

### Prerequisites

- Docker installed on your machine

### Getting Started

1. Clone the repository:
   ```bash
   git clone git@github.com:awet-dev/dockerized-php-app.git
2. Start the container:
   ```bash
   docker compose up -d 

### Add or Create your php app

- #### Existing application
  - From Git repository you can use this command to add your app to the application directory
    ```bash
      git clone <repository-url> application
- #### New Application
  - whether it is laravel or symfony you can create your project with the composer command

### Configure your environment variables 
> i.e symfony replace the variables starting with MYSQL_ with the configuration in compose.yaml file for db service, and so the same for mailer and so on
> ```bash 
> DATABASE_URL="mysql://MYSQL_USER:MYSQL_PASSWORD@db:3306/MYSQL_DATABASE?serverVersion=8.3.0&charset=utf8mb4"
>

### Check the web services  
- adminer: visit [adminer](http://localhost:8080)
- Mailer: visit [mailcatcher](http://localhost:1080)

Finally you are ready to go, enjoy coding
 