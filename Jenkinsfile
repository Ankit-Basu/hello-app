pipeline{
    agent any
    

    stages{
        stage('Clone') {
            steps {
                echo 'Cloning repository...'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...' 
            }
        }
        stage('Archive') {
            steps {
                archiveArtifacts 
                artifacts: 'target/*.jar'
            }
        }
    }
}