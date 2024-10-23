pipeline {
  agent any

  stages {
    stage ('build') {
      steps {
        echo 'Construction de l_application'
        sh 'npm install'
      }
    }

    stage ('test') {
      steps { 
        echo 'Test de l_application'
        sh 'npm test'
      }
    }
  }

  post {
    always {
      echo 'Pipeline d_integration continue finished'
    }
  }
}
