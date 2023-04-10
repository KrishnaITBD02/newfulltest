pipeline {
agent any

stages {

 stage('SonarQube analysis') {
  environment {
    scannerHome = tool 'sonarqube'
  }
  steps {
    withSonarQubeEnv('New_Test'){
      sh "${scannerHome}/bin/sonar-scanner -Dsonar.language=python"
    }
  }
}

}
}
