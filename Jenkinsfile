pipeline{
    agent any
    stages {
        stage ('FirstStage') {
            steps {
                echo "First Pipleline"
                sh "hostname -i"

            }
        }
        stage ('SecondStage') {
            agent {
                label 'java-slave'
            }
            steps {
                echo "Running on Java slave"
                sh "hostname -i"
            }
        }
    }
}
