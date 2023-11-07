pipeline {
    agent any

    stages {
        stage('Git Connect') {
            steps {
                sh 'rm -Rf jenkins'
                sh 'git clone https://github.com/testikung/jenkins.git'
                sh 'cd jenkins && ls -ltr'
                }
}
stage('Docker Image Creation')                                                                                                            {                                                                                                                                         steps{ 
                sh 'sudo docker ps'
                sh 'sudo docker images'
                sh 'sudo docker stop ikunginx01'
                sh 'sudo docker rm ikunginx01'
                sh 'sudo docker build -t ikunginx01 .'
                sh 'sudo docker run -dit --name ikunginx01 -p8022:80 ikunginx01'
                sh 'ls -ltr'
              
            }
        }
stage('Tag Image')                                                                                                                        {                                                                                                                                         steps{
               sh 'sudo docker image tag susigughnginx01 susigugh/susigughnginx01:1.0'                                                                }
        }
    }
}  
 
