pipeline{
    agent any
    tools {nodejs "node"}
        stages{       


         stage('build Application'){
            steps{
                script{
                    cmd.exe 'npm install'
                }
            }
        }
        
        stage('testing'){         
            steps{
                   script{
                      sh 'node test'
            }
                
            }
        }
        stage('deploy'){
            steps{
                   script{
               // gv_script.testApp()
               echo "Deploying Application..."
            }
            }
        }
    }

}
