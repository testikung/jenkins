pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                sh 'rm -Rf jenkins'
                sh 'git clone https://github.com/testikung/jenkins.git'
                sh 'cd jenkins && ls -ltr'
                sh 'sudo docker ps'
                sh 'sudo docker images'
                sh 'sudo docker build -t ikunginx01 .'
                sh 'sudo docker run -dit --name ikunginx01 -p8022:80 ikunginx01'
                sh 'ls -ltr'
              
            }
        }
    }
}
