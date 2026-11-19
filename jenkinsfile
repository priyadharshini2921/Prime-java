
pipeline {
    agent any

    triggers {
        githubPush()
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/priyadharshini2921/Prime-java.git'
            }
        }

        stage('Build') {
            steps {
                sh 'javac PrimeNumber.java'
            }
        }

        stage('Execute') {
            steps {
                sh 'echo 7 | java PrimeNumber'
            }
        }
    }
}
