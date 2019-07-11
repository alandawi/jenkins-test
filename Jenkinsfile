// comment
pipeline {
 agent any
 stages {
    stage('Checkout-git') {
        steps {
            git ls-remote -h git@github.com:alandawi/jenkins-test.git HEAD

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

