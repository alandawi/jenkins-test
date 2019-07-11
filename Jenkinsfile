// comment
pipeline {
 agent any
 stages {
     stage ('Clone') {
        steps {
            git branch: 'develop', url: "git@github.com:alandawi/jenkins-test.git"
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

