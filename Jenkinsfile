pipeline{
    agent any
    stages {
        stage ('FirstStage') {
            steps {
                echo "coming from build stage"
            }
        }
        stage('groovystage'){
            steps{
                script{
                // to define a variable
                def course = "Devops"
                println("Thanks for enrolling ${course} course")
                }
            }
        }

    }
}
