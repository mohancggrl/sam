pipeline{
    agent any
    environment{
        PATH = "/opt/maven/bin:$PATH"
    }
    stages{
        stage("Git_Checkout"){
            steps{
                git credentialsId: 'mohan', url: 'https://github.com/mohancggrl/hello-world-war.git'
            }
        }
        stage("Mvn Build") {
            steps {
                sh "mvn clean package"
            }
        }
    }
}
