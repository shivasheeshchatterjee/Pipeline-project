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
}
