pipeline {
    agent any

    tools {
        
        maven "apache-maven-3.9.2"
    }

    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/mulesoft2030/CubeGenerator.git'
            }
		}
		stage('mvn version') {
            steps {
               bat 'mvn --version'
            }
		}
		stage('mvn validate') {
            steps {
               bat 'mvn validate'
            }
		}	
        

	
	}
}