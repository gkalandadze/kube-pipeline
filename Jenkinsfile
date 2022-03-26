pipeline {
  agent {
    kubernetes {
      yamlFile "pod-template.yaml"
    }
  }
  tools {
    maven 'Maven 3.8.5'
  }
  stages {
    stage('First Stage') {
      steps {
        sh 'mvn -v'
      }
    }
  }
}
