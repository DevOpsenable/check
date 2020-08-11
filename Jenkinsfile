pipeline {
    agent any
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
