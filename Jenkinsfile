pipeline{
    agent {
        label "java-slave"
    }
    tools {
        maven 'mvn'
        jdk 'JDK-21'
    }

    environment {
        APPLICATION_NAME = 'eureka'
    }
    stages{
        stage("build"){
            steps {
                echo "***building eureka application***"
                sh "mvn clean"
            }
        }
        stage("sonarscan"){
            steps {

            }
        }
    }

}