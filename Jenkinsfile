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
  post {
    success {
      echo "Pipeline completed successfully"
    }
  }
  tools {
    maven 'Maven 3.8.5'
  }
}
