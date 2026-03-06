pipeline {
    agent any
    
    parameters {
        string(name: 'PROJECT_NAME', defaultValue: 'agileCat', description: 'Project Name')
        string(name: 'BUILD_ID', defaultValue: '505', description: 'Numeric Build ID')
        string(name: 'APP_NAME', defaultValue: 'CatApp', description: 'Application Name')
        string(name: 'VERSION', defaultValue: 'v2.0', description: 'Version Number')
    }

    stages {
        stage('Version 4: Store All Parameters') {
            steps {
                // Task 1: Checkout the latest commit from GitHub
                checkout scm
                
                // Task 2: Display all parameter values in the console output
                echo "--- Parameter Values ---"
                echo "Project: ${params.PROJECT_NAME}"
                echo "Build ID: ${params.BUILD_ID}"
                echo "App Name: ${params.APP_NAME}"
                echo "Version: ${params.VERSION}"
                
                // Task 3: Store the parameter values inside parameters.txt file
                bat "echo PROJECT_NAME: ${params.PROJECT_NAME} > parameters.txt"
                bat "echo BUILD_ID: ${params.BUILD_ID} >> parameters.txt"
                bat "echo APP_NAME: ${params.APP_NAME} >> parameters.txt"
                bat "echo VERSION: ${params.VERSION} >> parameters.txt"
                
                // Display the file contents to verify
                bat "type parameters.txt"
            }
        }
    }
}