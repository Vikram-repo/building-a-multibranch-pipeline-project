pipeline {
    agent {
      tool {
         nodejs 'node-lts'
    }
    environment {
        CI = 'true'
    }
    stages {
        stage ('build') {
            steps {
                sh 'npm install'
            }
        }
        stage ('test') {
            steps {
                sh './jenkins/scripts/test.sh'
            }
        }
    }
}
