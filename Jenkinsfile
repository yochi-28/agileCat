pipeline {
    agent any
    
    // Task 2: Define a string parameter named PROJECT_NAME
    parameters {
        string(name: 'PROJECT_NAME', defaultValue: 'agileCat', description: 'Enter the project name')
    }

    stages {
        stage('Version 1: String Parameter') {
            steps {
                // Task 1: Checkout the project from GitHub
                checkout scm
                
                // Task 3: Display the value of the parameter in the Jenkins console
                echo "The Project Name parameter is: ${params.PROJECT_NAME}"
            }
        }
    }
}