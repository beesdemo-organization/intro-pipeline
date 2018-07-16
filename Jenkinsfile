pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('Say Hello') {
      steps {
        echo "Where are my pants? ${MY_NAME}"
        echo "${TEST_USER_USR}"
        echo "${TEST_USER_PSW}"
        sh 'java -version'
      }
    }
  }
  environment {
    MY_NAME = 'Phil McKraken'
    TEST_USER = credentials('test-user')
  }
}