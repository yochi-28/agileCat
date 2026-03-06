pipeline {
    agent any
    stages {
        stage('Version 1: Workspace Info') {
            steps {
                // Task 1: Checkout source code from GitHub
                checkout scm
                
                // Task 2: Display the Jenkins workspace path using %WORKSPACE%
                bat 'echo The workspace path is: %WORKSPACE%'
                
                // Task 3: Print a message indicating execution has started
                echo 'Pipeline execution has started.'
            }
        }
    }
}