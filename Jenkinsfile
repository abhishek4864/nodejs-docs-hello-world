pipeline{
    agent any
    environment {
        NEW_VERSION='1.3.0'
        //SERVER_CRED=credentials('<id of cred in GUI>')
    }
    parameters{
        string(name: 'Version',  defaultValue:'1.0',description:'version to deploy')
        choice(name:'Version',choices:['1.0','1.1','1.2'],description:'choose version')
        booleanParam(name:'testParam',defaultValue:'true',description:'decider')
    }
    stages{       
         stage('checkout'){
            //  when{
            //      expression{
            //          BRANCH_NAME=="dev" $$ CODE_CHANGES==true
            //      }
             //}
            steps{
                echo "checking out the repo version ${NEW_VERSION}"
            }
        }
        stage('testing'){
            when{
                expression{
                    params.testParam==true
                }
            }
            steps{
                echo "testing the code ${params.Version}"
            }
        }
        stage('deploy'){
            steps{
                echo "deploying the code"
                //echo "deploying with ${SERVER_CRED}"
            }
        }
    }

}
