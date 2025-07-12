pipeline {
    agent{
        label 'java-slave'

    }
    environment {
        Today_Day = 'Saturday'
    }
    stages{
        stage('Build Stage'){
            when{
                environment name: 'Today_Day', value: 'Saturday'
            }
            steps{
                echo "When Example"
            }
        }
    }
}
