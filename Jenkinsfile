pipeline {
    agent any
    environment {
           BRANCH_NAME = 'master'
               }
    parameters {
              name: 'PARAM1'
    }
    stages {
        stage('Build') {
            steps {
                echo 'H!!ey HEY'
                echo "${name}"     
            }
        }
    }
}
