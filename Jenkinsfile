pipeline {
   
    agent any
   
    stages {

        stage('get code from github') {
            steps {
                echo 'Pulling...';
                git branch: 'main',
                url : 'https://github.com/Pseudoisalreadytaken/exoJenkinsNgrok.git';
            }

            post {
                success {
                    echo "====++++success++++===="
                }
               
                failure {
                    echo "====++++failed++++===="
                }
            }
           
        }
           
    }
}