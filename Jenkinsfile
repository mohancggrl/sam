pipeline{
    agent any
    environment{
        PATH = "/opt/maven/bin:$PATH"
    }
    stages{
        stage("Mvn Build") {
            steps {
                sh "mvn clean package"
            }
        }
    }
}
