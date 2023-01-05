pipeline {
   
    agent any
   
    stages {

        stage('get code from github + web hook') {
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