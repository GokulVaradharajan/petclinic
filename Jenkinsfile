pipeline 
{
    agent any
    
    tools
    {
        maven "MAVEN_HOME"
    }
    stages{
        stage('Build'){
            steps{
                git 'https://github.com/GokulVaradharajan/petclinic.git'
                bat "mvn clean install package"
            }
        }    
    }
}
