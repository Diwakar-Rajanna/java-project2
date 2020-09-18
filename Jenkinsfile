pipeline {
	agent master
	stages {
		stage ('java clone and build') {
			steps {
				sh ''' cd /home/ec2-user/
				git clone 'https://github.com/Diwakar-Rajanna/java-project2.git'
				cd java-project2
				mvn clean install
				cd target 
				sh 'sleep 10'
				'''
			}	
		}
		stage ('c clone ') {
			steps {
				sh ''' cd /home/ec2-user/
				git clone 'https://github.com/Diwakar-Rajanna/c-project.git'
				cd c-project
				make
				sh 'sleep 10'
			}	
		}
			}	
		}
	}
