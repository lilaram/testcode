node {
  stage('SCM') {
    checkout scm
  }
  stage('SonarQube Analysis') {
    
    def scannerHome = tool 'sonarscanner';
    withSonarQubeEnv('SonarQubeServer') {
      '''
      sh ${scannerHome}/bin/sonar-scanner \
       -D sonar.projectKey=testyamlfiles \
       -D sonar.projectName=testyamlfiles \
       -D sonar.host.url=http://18.193.109.212:9000 \  
       -D sonar.login=sqp_d0e764300d09cdbe5875df9f4b0cbf234a231b9f \
       '''
      
    }
  }
}
