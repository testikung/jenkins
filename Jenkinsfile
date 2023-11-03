pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello Ikung'
                sh 'pwd'
                sh 'ls -ltr'
                sh 'touch a.txt'
                sh 'ls -ltr'
                sh 'rm -Rf jenkins'
                sh 'git clone https://github.com/testikung/jenkins.git'
                sh 'cd jenkins && ls -ltr'
                sh 'ls -ltr'
            }
        }
    }
}
