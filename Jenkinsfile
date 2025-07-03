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
                def course = "k8s"
                if (course == "Devops")
                println("Thanks for enrolling")
                
                else 
                println("Do enroll")
                //println("Thanks for enrolling ${course} course")
                }
            }
        }

    }
}
