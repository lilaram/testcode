pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                sh "ansible --version"
                sh "sonar-scanner"
            }
        }
    }
}
