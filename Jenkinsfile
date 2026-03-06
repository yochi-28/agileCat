pipeline {
    agent any
    stages {
        stage('Version 2: List Workspace and Time') {
            steps {
                // Task 1: Checkout the updated repository
                checkout scm
                
                // Task 2: Use the 'dir' command to list all files and folders
                bat 'dir'
                
                // Task 3: Display the current system time using BAT command
                bat 'echo Current system time: %time%'
            }
        }
    }
}