Pipeline{
    agent{
        label 'java-slave'
    }
    environment{
        deploy_to = 'production'
    }
    stages{
        Stage('deploytodev'){
            steps{
                echo "Deploying to dev env"
            }
        }
        stage ('proddeploy')
        {
            when {
                allOf{
                     branch 'production'
                     environment name:'deploy_to', value: 'production'
                }
                
            }
            steps{
                echo " deploying to prod  "
            }
        }
    }
}
