pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                sh 'rm -Rf jenkins'
                sh 'git clone https://github.com/testikung/jenkins.git'
                sh 'cd jenkins && ls -ltr'
                sh 'sudo docker ps'
                sh 'ls -ltr'
              
            }
        }
    }
}
