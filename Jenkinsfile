pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build message'
      }
    }

    stage('Test1') {
      parallel {
        stage('Test1') {
          steps {
            echo 'Test message 1'
          }
        }

        stage('Test2') {
          steps {
            echo 'Test message 2'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy message'
      }
    }

  }
  environment {
    env_key1 = 'env_var1'
    more_env_keys = 'more_env_vars'
  }
}