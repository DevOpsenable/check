pipeline {
    agent any
    environment {
           BRANCH_NAME = 'master'
               }
    parameters {
              name: 'PARAM1'
    }
    stages {
        stage('build') {
            steps {
                echo 'Hey HEY'
                echo "${name}"     
            }
        }
    }
}
