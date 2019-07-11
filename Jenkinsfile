// comment
pipeline {
 agent any
 stages {
    stage('Checkout-git') {
            steps{
                git poll: true, url: 'git@github.com:alandawi/jenkins-test.git'
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

