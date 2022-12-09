pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                sh "ansible --version"
                sh "/home/ubuntu/sonar-scanner-4.7.0.2747-linux/sonar-scanner -h"
            }
        }
    }
}
