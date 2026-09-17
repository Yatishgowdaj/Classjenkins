pipeline {
    agent any
    stages{
        stage("Build"){
            steps{
                echo "Building the project..."
            }
        }
        stage("Parallel Test"){
            parallel {
                stage("Unit Test"){
                    steps{
                        echo "Running Unit Tests..."
                    }
                }
                stage("Integration Test"){
                    steps{
                        echo "Running Integration Tests..."
                    }
                }
            }
        }

    }
}