node {
  stage('SCM') {
    checkout scm
  }
  stage('SonarQube Analysis') {
    
    def scannerHome = tool 'sonarscanner';
    withSonarQubeEnv('SonarQubeServer') {
      
      " sh ${scannerHome}/bin/sonar-scanner "
      
      
    }
  }
}
