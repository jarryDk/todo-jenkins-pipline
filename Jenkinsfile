pipeline {
    agent any 
    stages {
        stage('Setup') { 
            steps {
                sh 'mvn -version' 
            }
        }
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}