pipeline{
    agent any
    stages{
        stage('Git clone'){
            steps{
                git branch: 'main', url: 'https://github.com/franci-hub/HelloWorld_Springboot.git'
            }
        }
        stage('Maven Test'){
            steps{
                bat 'mvn test'
            }
        }
        stage('Maven Build'){
            steps{
                bat 'mvn package'
            }
        }
        stage('Maven Deploy'){
            steps{
                echo "Test Deploy Maven"
            }
        }
    }
}
