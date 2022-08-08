pipeline 
{
    agent any
    
    tools
    {
        maven "M3"
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
