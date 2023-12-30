pipeline {
    agent any 
    stages {
        stage('Compile and Clean') { 
            steps {
                sh "rm -rf maven-project"
            }
        }
        stage('Test') { 
            steps {
                sh "mvn test"
            }
        }
        stage('Deploy') { 
            steps {
                sh "mvn package"
            }
        }
    }
}
