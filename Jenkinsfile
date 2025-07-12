pipeline{
    agent{
        label 'java-slave'
    }
    environment{
        deploy_to = 'production'
    }
    stages{
        stage('deploytodev'){
            steps{
                echo "Deploying to dev env"
            }
        }
        stage ('proddeploy')
        {
            when {
                allOf {
                     branch 'main'
                     environment name:'deploy_to', value: 'production'
                }
                
            }
            steps {
                echo " deploying to prod  "
            }
        }
    }
}
