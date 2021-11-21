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
                bat """
                   node test
                    """

                
            }
        }
        stage('deploy'){
            steps{
            steps{
                echo "deploying application"
 

                
            }
            }
        }
    }

}
