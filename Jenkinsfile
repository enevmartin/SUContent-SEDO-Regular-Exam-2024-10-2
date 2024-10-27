pipeline {
    agent any 

    stages {
        stage('Build') {
            steps {
                script {
                    echo 'Building the application...'
                    // Replace with your build command, for .NET 6
                    sh 'dotnet build --configuration Release'
                }
            }
        }
        stage('Test') {
            steps {
                script {
                    echo 'Running tests...'
                    // Replace with your test command
                    sh 'dotnet test --no-build --configuration Release'
                }
            }
        }
    
}
