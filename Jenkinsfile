pipeline {
    agent any
    
    // Task 2: Define two parameters named APP_NAME and VERSION
    parameters {
        string(name: 'APP_NAME', defaultValue: 'CatApp', description: 'Enter the Application Name')
        string(name: 'VERSION', defaultValue: 'v1.0', description: 'Enter the Version Number')
    }

    stages {
        stage('Version 3: Multiple Parameters') {
            steps {
                // Task 1: Checkout the latest repository version
                checkout scm
                
                // Task 3: Display a combined message containing both parameter values
                echo "Deploying Application: ${params.APP_NAME} | Version: ${params.VERSION}"
            }
        }
    }
}