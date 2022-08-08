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
                sh "mvn clean install package"
            }
        }    
    }
}
