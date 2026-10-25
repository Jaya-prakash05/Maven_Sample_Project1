pipeline{
    agent any
    stages{
        stage("build"){
            steps{
                git "https://github.com/Jaya-prakash05/Maven_Sample_Project1.git"
            }
        }
        stage("maven"){
            steps{
                bat '''
                mvn package
                '''
            }
        }
        stage("excute"){
            steps{
                bat 'java -jar target/java-project2-1.9.jar'
            }
        }
    }
}
