pipeline {
    agent any 

     environment {
        AWS_ACCESS_KEY_ID     = credentials('secret-key-for-s3')
        AWS_SECRET_ACCESS_KEY = credentials('secret-access-key-for-s3')
    } 
    stages {
        stage('1st') {
            steps {
                echo "Hi!"
                sh 'aws s3 cp ./ s3://mybucket-kanstantsin/jenkinsindex.html'
            }
        }
        
    }   
    
}
