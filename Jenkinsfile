pipeline{
    agent any
    stages{
        stage('Clean Stage'){
            steps{
                echo "Cleaning the previous build."
                sh "mvn clean"
            }
        }
        stage('Test'){
            steps{
                echo "Testing if the build is okay"
                sh "mvn test"
            }
        }
        stage('Package'){
            steps{
                echo "Packaging the build"
                sh "mvn package"
            }
        }
    }
}