pipeline{
    agent any
    stages{
        stage('Git clone'){
            steps{
                git branch: 'main', url: 'https://github.com/franci-hub/HelloWorld_Springboot.git'
            }
        }
        stage('Maven Build'){
            steps{
                bat 'mvn package'
            }
        }
        stage('Create DockerImage'){
            steps{
               bat 'docker build -t franci/springboot:latest .'
            }
        }
    }
}
