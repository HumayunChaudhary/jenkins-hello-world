pipeline {
    agent any

    tools {
        maven 'maven-398'
		jdk 'jdk-17'
    }

    stages {

        stage('checkout') {
            steps {
                git url: 'https://github.com/HumayunChaudhary/jenkins-hello-world.git', branch: 'main'
            }
        }

        stage('build') {
            steps {
                sh 'mvn clean package -DskipTests'
            }
        }

        stage('test') {
            steps {
                sh 'mvn test'
            }
        }

    }
}
