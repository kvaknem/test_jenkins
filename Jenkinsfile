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
            input {
                message "Should we continue?"
                ok "Yes, we should."
                submitter "alice,bob"
                parameters {
                    string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
                }
            steps {
                sh 'ls -lah'
                 echo "Hello, ${PERSON}, nice to meet you."
            }
        }
        stage('Deploy') { 
            steps {
                sh 'pwd' 
            }
        }
    }
}
