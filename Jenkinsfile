pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o PES2UG20CS246-1 wrong.cpp'
                echo "Build Successful"
            }
        }
        stage('Test') {
            steps {
                sh './PES2UG20CS246-1'
            }
        }
    }
    post {
        always {
            echo 'Pipeline has been completed.'
        }
        failure {
            echo 'Oops! Pipeline has failed.'
        }
    }
}

