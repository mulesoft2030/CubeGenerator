pipeline {
    agent any

    tools {
        
        maven "apache-maven-3.9.2"
    }

    stages {
        stage('Clone') {
            steps {
                git branch: 'main', credentialsId: 'syedmulesoft2030', 'https://github.com/mulesoft2030/CubeGenerator.git'
            }
		}
		stage('mvn deploy') {
            steps {
                 configFileProvider(
                    [configFile(fileId: 'settings.xml', target: 'settings.xml')]) {
                    bat 'mvn clean deploy -s settings.xml'
                }
                
			}    
		}	
        

	
	}
}
