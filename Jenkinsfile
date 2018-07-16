pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('Say Hello') {
      steps {
        echo "Where are my pants? ${MY_NAME}"
        sh 'java -version'
      }
    }
  }
  environment {
    MY_NAME = 'Phil McKraken'
  }
}