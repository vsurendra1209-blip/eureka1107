pipeline{
    agent {
        label "java-slave"
    }
    tools {
        maven 'maven-3.9.16'
    }
    stages{
        stage("build"){
            steps {
                sh "mvn clean"
            }
        }
    }

}