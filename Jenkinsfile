pipeline{
    agent any
    tools {nodejs "node"}
        stages{       


         stage('build Application'){
            steps{
                cmd.exe 'npm install'
                //script{
                  //  cmd.exe 'npm install'
               // }
            }
        }
        
        stage('testing'){         
            steps{
                   script{
                      cmd.exe 'node test'
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
