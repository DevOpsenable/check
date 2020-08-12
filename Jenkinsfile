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
                echo "H!!ey HEY"
                echo "${name}"     
            }
        }
    }
}
