pipeline {
    agent any
    stages {
        stage("Compile") {
            steps {
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
