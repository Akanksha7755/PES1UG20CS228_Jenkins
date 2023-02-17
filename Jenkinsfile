pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ temp.cpp -o temp'
                 build job: 'PES1UG20CS228-1', wait: false
                 echo 'Successfully built -Akanksha'
            }
        }

        stage('Test') {
            steps {
                sh 'cat temp.cpp'
                echo 'Test -Akanksha'
            }
        }

        stage('Deploy') {
            steps {
               
                echo 'Successfully Deployed -Akanksha'
            }
        }
    }

    post {
        failure {
            
                echo 'Pipeline Failed'
          
        }
    }
}
