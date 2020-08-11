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
          when {
             expression { 
                      BRANCH_NAME == name
                        }
                }        
           steps {
                echo "Hey HEY"
                echo "${name}"
                sh "testm.sh"      
            }
        }
    }
}
