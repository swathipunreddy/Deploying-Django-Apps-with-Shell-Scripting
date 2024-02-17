Simplifying Deployment: Deploying Django Apps with Shell Scripting

Introduction:
In this project, I've developed a deployment script using shell scripting techniques to simplify the deployment process for Django applications. The deployment script automates various tasks involved in deploying a Django app, such as cloning the code, installing dependencies, performing necessary restarts, and deploying the application using Docker.

Explanation:

    Cloning the Code:
    The first step in the deployment process is to clone the Django app code from the GitHub repository. The script checks if the code directory already exists. If not, it clones the code using the git clone command.

    Installing Dependencies:
    After cloning the code, the script installs the required dependencies for running the Django app. This includes packages like Docker, nginx, and docker-compose. It uses apt-get to update the package list and install the dependencies.

    Performing Necessary Restarts:
    Once the dependencies are installed, the script performs necessary restarts to ensure that Docker and nginx are configured properly. It changes the ownership of the Docker socket and enables and restarts Docker and nginx services.

    Deploying the Application:
    Finally, the script builds and deploys the Django app using Docker. It builds a Docker image for the app using the docker build command and then runs the app in a Docker container using the docker-compose up command.

Conclusion:
By automating the deployment process with a shell script, we've simplified the deployment of Django applications. The script handles various tasks involved in deployment, reducing manual effort and potential errors. With this script, deploying Django apps becomes faster, more reliable, and easier to manage.
