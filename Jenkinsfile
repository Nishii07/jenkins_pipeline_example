pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''echo \'hi\'
pwd
ls -l'''
      }
    }

    stage('test1') {
      parallel {
        stage('test1') {
          steps {
            echo 'hello nishi'
          }
        }

        stage('test2') {
          steps {
            sh '''date
cal'''
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'code has been deployed'
        sh 'echo "success"'
      }
    }

  }
}