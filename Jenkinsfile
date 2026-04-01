pipeline {
	agent any
	
	tools {
		'maven-398'
	}
	
	stages {
		
		stage('checkout') {
			git url: 'https://github.com/HumayunChaudhary/jenkins-hello-world', branch: 'main'
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
