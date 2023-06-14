pipeline {
    agent any

    tools {
        
        maven "apache-maven-3.9.2"
    }

    stages {
        
           	
        stage('mvn version') {
            steps {
                bat 'mvn --version'
            }
		}
		
	    stage('Clone') {
            steps {
                git credentialsId: 'syedmulesoft2030', url: 'https://github.com/mulesoft2030/CubeGenerator.git'
            }
		}

	
	}
}
