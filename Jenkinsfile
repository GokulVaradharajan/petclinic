pipeline {
agent any
    tools {
        maven 'MAVEN_PATH'
        jdk 'jdk8'
    }
    stages {
        stage("Tools initialization") {
            steps {
                sh "mvn --version"
                sh "java -version"
            }
        }
        stage("Checkout Code") {
            steps {
                git branch: 'master',
                url: "https://github.com/GokulVaradharajan/petclinic.git"
            }
        }
        stage("Building Application") {
            steps {
               sh "mvn clean package"
            }
        }
    }
}
