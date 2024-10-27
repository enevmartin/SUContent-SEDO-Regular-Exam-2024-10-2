pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Build the .NET 6 application
                sh 'dotnet build --configuration Release'
            }
        }
        stage('Run Tests') {
            steps {
                // Run all tests (unit and integration)
                sh 'dotnet test --no-build --configuration Release'
            }
        }
    }
}
