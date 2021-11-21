pipeline{
    agent any
    tools {nodejs "node"}
        stages{       


         stage('build Application'){
            steps{
                echo "Building application"
                bat """
                    npm install
                    """
            }
        }
        
        stage('testing'){         
            steps{
                echo "Testing application"


                
            }
        }
        stage('deploy'){
         
            steps{
                echo "deploying application"
 

                
            
            }
        }
    }

}
