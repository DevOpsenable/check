pipeline {
agent any
stages {
  stage("Use alias command"){
    steps { 
        sh '''
          alias foo="bar"
          foo
        '''
    }
  }
}}
