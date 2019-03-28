pipeline {
      agent any
      stages {
        stage('Build') {
            steps {
                bat 'mvn -v'
            }
        }
    }
      
      
      
      post{

      always{
       echo 'Finished--------------------------'     
      }
}

      
      
}

