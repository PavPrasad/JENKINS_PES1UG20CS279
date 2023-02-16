pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ tester.cpp -o tester'
                 build job: 'PES1UG20CS279-1', wait: false
                 echo 'Build by CS279 successful'
            }
        }

        stage('Test') {
            steps {
                sh 'cat tester.cpp'
                echo 'Test by CS279 successful'
            }
        }

        stage('Deploy') {
            steps {
               sh 'skdjfskf'
                echo 'Deploy by CS279 successful'
            }
        }
    }

    post {
        failure {
            
                echo 'Pipeline Failed'
          
        }
    }
}
