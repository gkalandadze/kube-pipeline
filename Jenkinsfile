pipeline {
  agent {
    kubernetes {
      yamlFile 'pod-template.yaml'
    }

  }
  stages {
    stage('First Stage') {
      steps {
        sh 'mvn -v'
      }
    }

    stage('Second Stage') {
      steps {
        sh 'hostname'
      }
    }

  }
  tools {
    maven 'Maven 3.8.5'
  }
}