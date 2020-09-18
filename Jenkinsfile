pipeline {
	agent none
 
	stages {
		stage ('STAGE 1') {
			agent { label 'slave1' }
			steps {
				git 'https://github.com/ranjitha-12345/ccode.git'
				sh 'make'
				
			}	
		}
		stage ('STAGE 2') {
			agent { label 'slave2' }
			steps {
			
				git 'https://github.com/ranjitha-12345/Test-1.git'
				sh 'mvn clean install'
			}	
		}
		
	}
}
