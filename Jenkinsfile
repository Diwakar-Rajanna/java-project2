pipeline {
	agent any
  environment{
  PATH = /usr/share/man/man1/:$PATH
  }
	stages {
		stage ('git_clone') {
			steps {
				git 'https://github.com/Diwakar-Rajanna/java-project2.git'
				sh 'sleep 10'
			}	
		}
		stage ('build') {
			steps {
				sh 'mvn clean install '
				sh 'sleep 10'
			}	
		}
			}	
		}
	}
}
