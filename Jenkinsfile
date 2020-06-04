
pipeline {
    agent { docker { image 'maven:3.6.3' } }
    stages {
        stage('Build') {
            steps {
                sh 'mvn --version'
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
