pipeline {
      agent any
      stages {
        stage('Build') {
            steps {
                bat 'mvn -v'
                  input "Does the buil environment look ok?"
            }
        }
    }
      
      
      
      post{

      always{
       echo 'Finished--------------------------'     
      }
      success {
            echo 'I succeeeded!'
            
        }
        unstable {
            echo 'I am unstable :/'
        }
        failure {
            echo 'I failed :('
        }
        changed {
            echo 'Things were different before...'
        }
            
            
            
            
            
}

      
      
}

