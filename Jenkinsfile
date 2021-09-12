pipeline {
    agent any 
    stages {
        stage('Setup') { 
            tools {
                   jdk "jdk17"
                }
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