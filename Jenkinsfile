pipeline{
    agent any
    tools {nodejs "node"}
        stages{       


         stage('build Application'){
            steps{
               // cmd.exe 'npm install'
                cmd_exec('"npm install"')
                //script{
                   // cmd.exe 'npm install'
                //}
            }
        }
        
         stage('Test Application'){
            steps{
               // cmd.exe 'npm install'
                cmd_exec('"node test"')
                //script{
                   // cmd.exe 'npm install'
                //}
            }
        }
         stage('Deploy Application'){
            steps{
               // cmd.exe 'npm install'
                cmd_exec('echo "deploy apllication..."')
                //script{
                   // cmd.exe 'npm install'
                //}
            }
        }
    }

}
