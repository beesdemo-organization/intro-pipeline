pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('Say Hello') {
      steps {
        echo "Where are my pants? I'm looking at you ${params.Name}"
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
  parameters {
    string(name: 'Name', defaultValue: 'whoever you are', description: 'Who should I say hi to?')
  }
}