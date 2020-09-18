pipeline {
	agent none
 
	stages {
		stage ('STAGE 1') {
			agent LABEL: slave1
			steps {
				echo 'This is slave for ccode node with STAGE 1'
				sh 'sleep 10'
			}	
		}
		stage ('STAGE 2') {
			agent LABEL: slave2
			steps {
				echo 'This is slave for java with STAGE 2'
				sh 'sleep 10'
			}	
		}
		stage ('STAGE 3') {
			steps {
				echo 'This is slaveforc with STAGE 3'
				sh 'sleep 5'
			}	
		}
		stage ('STAGE 4') {
			steps {
				echo 'This is master with STAGE 4'
				sh 'sleep 5'
			}	
		}
	}
}
