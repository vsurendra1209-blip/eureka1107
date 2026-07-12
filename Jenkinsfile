pipeline{
    agent {
        label "java-slave"
    }
    tools {
        maven 'mvn'
    }
    stages{
        stage("build"){
            steps {
                sh "mvn clean"
            }
        }
    }

}