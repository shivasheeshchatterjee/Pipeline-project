pipeline {
    agent any
    environment{
        VERSION_NAME="Validation"
    }
    stages {
        stage("Compile") {
            steps {
                echo "Version: ${env.VERSION_NAME}"
                bat 'javac Test.java'
            }
        }
        stage("Run") {
            steps {
                bat 'java Test'
            }
        }
    }
    
    post {
        always {
            echo 'It will run always'
        }
        success {
            echo 'It is a success'
        }
        failure {
            echo 'Too bad it failed'
        }
    }
}
