pipeline {
	agent none
 
	stages {
		stage ('STAGE 1') {
			agent { label 'slave1' }
			steps {
				echo 'This is slave for ccode node with STAGE 1'
				sh 'sleep 15'
			}	
		}
		stage ('STAGE 2') {
			agent { label 'slave2' }
			steps {
				echo 'This is slave for java with STAGE 2'
				sh 'sleep 15'
			}	
		}
		stage ('STAGE 3') {
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
		}
	}
}
