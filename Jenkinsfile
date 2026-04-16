pipeline{
    agent any
    
    stages{
        stage('Clone'){
            steps {
                echo 'Cloning successful'
            }
        }
    }
    stages{
        stage('Build') {
            steps {
                bat 'mvn clean package'
            }
        }
    }
}