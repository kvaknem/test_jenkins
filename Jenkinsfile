pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                sh 'hostname'
                sh 'whoami'
            }
        }
        stage('Test') { 
            steps {
                sh 'ls -lah'
            }
        }
        stage('Deploy') { 
            steps {
                sh 'pwd' 
            }
        }
    }
}
