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
      success {
            echo 'I succeeeded!'
            mail to: 'rajeshkummetha@gmail.com',
             subject: "success with Pipeline: ${currentBuild.fullDisplayName}",
             body: "all is well ${env.BUILD_URL}"
            
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

