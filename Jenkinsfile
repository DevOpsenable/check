pipeline {
    agent any
    parameters {
        string(name: 'PARAM1', description: 'Param 1?')
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
                echo "${params}"
                sh testm.sh      
            }
        }
    }
}
