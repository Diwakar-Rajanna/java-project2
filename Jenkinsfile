pipeline {
	agent none

	stages {
		stage ('C Project') {
			agent { label 'java' }
			steps {
			  	git 'https://github.com/GuruDeshmukh/Jenkinsproject2.git'
					sh 'make'
			}
		}
		stage ('Java Project') {
			agent { label 'java-1' }
			steps {
				git 'https://github.com/GuruDeshmukh/Test-1.git'
				sh 'mvn clean install'
			}
		}
		
	}
}
