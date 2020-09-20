pipeline {
	agent none
 
	stages {
		 
			 
				stage ('ccode') {
					agent { label 'node1-c' }
					steps {
						git 'https://github.com/Shruthi-github123/ccode.git'
						sh 'make'
				
					}	
				}
				stage ('java') {
					agent { label 'node2-maven' }
					steps {
			
					git 'https://github.com/Shruthi-github123/Test-1.git'
					sh 'mvn clean install'
					}	
				}
			
		
		
	 }
 }
