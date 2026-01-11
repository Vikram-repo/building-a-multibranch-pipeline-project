pipeline {
    agent any
 environment {
    CI = 'true'
 }
 stages{
    stage ('build') {
        steps {
            sh 'npm install'
        }
    }
    stage ('test') {
        steps {
            sh './jenkins/scrips/test.sh'
        }
    }
 }
}
