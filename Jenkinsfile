pipeline {
    agent any
    parameters {
        string(BRANCH_NAME: 'PARAM1', description: 'Param 1?')
    }
    stages {
        stage('build') {
          when {
              expression { 
                        BRANCH_NAME == BRANCH_NAME
                        }
                }        
          steps {
                echo "${params}"
                sh testm.sh                
                script {
                    def myparams = params + string(name: 'MYPARAM', value: "${params.MYPARAM}")
                    build job: 'downstream-pipeline-with-params', parameters: myparams
                }    
            }
        }
    }
}
