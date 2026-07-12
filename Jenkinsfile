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
                echo "***building ${env.APPLICATION_NAME} application***"
                sh "mvn clean -DskipTests=true"
            }
        }
        stage("sonarscan"){
            steps {
                echo "***sonrscans***"
            }
        }
    }

}