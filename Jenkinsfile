// comment
pipeline {
 agent any
 stages {
    stage('Checkout-git') {
            steps{
                git url: 'git@github.com:alandawi/jenkins-test.git'
            }
    }
    stage('Run Build') {
        steps {
            sh '''
                yarn build
            '''
        }
    }
  }
}

