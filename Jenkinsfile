pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Biuld...'
            }
        }
        
        stage('Test') {
            steps {
                echo 'Test ....'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'deploy....'
            }
        }
    }
     post {
                // If Maven was able to run the tests, even if some of the test
                // failed, record the test results and archive the jar file.
                always {
            emailext body: 'A Test EMail',to:'salikramchadar@gmail.com', subject: 'Test'
        }
            }
    
}
