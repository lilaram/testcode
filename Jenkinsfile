node {
  stage('SCM') {
    checkout scm
  }
  stage('SonarQube Analysis') {
    sh  "echo ${WORKSPACE}"
    sh "ls -ltr"
    sh "id"
    def scannerHome = tool 'sonarscanner';
    withSonarQubeEnv('SonarQubeServer') {
      sh "${scannerHome}/bin/sonar-scanner"
    }
  }
}
