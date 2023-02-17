pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ error.cpp -o error'
                 build job: 'PES1UG20CS163-1', wait: false
                 echo 'Build by CS163 successful'
            }
        }

        stage('Test') {
            steps {
                sh 'cat temp.cpp'
                echo 'Test by CS163 successful'
            }
        }

        stage('Deploy') {
            steps {
               
                echo 'Deploy by CS163 successful'
            }
        }
    }

    post {
        failure {
            
                echo 'Pipeline Failed'
          
        }
    }
}
