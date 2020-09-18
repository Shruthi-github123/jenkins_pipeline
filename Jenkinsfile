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
		/*stage ('STAGE 3') {
			agent { label 'slave1' }
			steps {
				echo 'This is slaveforc with STAGE 3'
				sh 'sleep 15'
			}	
		}
		stage ('STAGE 4') {
			agent { label 'master' }
			steps {
				echo 'This is master with STAGE 4'
				sh 'sleep 15'
			}	
		}*/
	}
}
