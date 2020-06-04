
pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo "Build"
            }
        }
        stage('Test') {
              steps {
                  echo "Test"
              }
        }
        stage('Integration Test') {
              steps {
                  echo "Integration Test"
              }
        }
    }
    post {
        always {
            echo 'I am run always'
        }
        success {
             echo 'I am run when you are successful'
        }
        failure {
             echo 'I am run when you fail'
        }
    }
}
