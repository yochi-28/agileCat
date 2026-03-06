pipeline {
    agent any
    
    // Task 2: Define a numeric parameter named BUILD_ID
    parameters {
        string(name: 'BUILD_ID', defaultValue: '101', description: 'Enter the numeric Build ID')
    }

    stages {
        stage('Version 2: Numeric Parameter') {
            steps {
                // Task 1: Checkout the updated repository version
                checkout scm
                
                // Task 3: Save the BUILD_ID value inside buildinfo.txt and read it
                bat "echo ${params.BUILD_ID} > buildinfo.txt"
                bat "type buildinfo.txt"
            }
        }
    }
}