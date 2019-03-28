pipeline {
      agent any
      stages {
        stage('Buil') {
            steps {
                bat 'mvn -v'
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

