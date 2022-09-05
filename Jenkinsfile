pipeline {
	// agent any
	agent { docker { image 'maven:latest' } }
	stages {
		stage('Build'){
			steps{
				sh 'mvn --version'
				echo "Build"
			}
		}
		stage('Test'){
			steps{
				echo "Test"
			}
		}
		stage('Integration Test'){
			steps{
				echo "Integration Test"
			}
		}
		
	} 
	post {
		always {
			echo "I am Awesome"
		}
		success {
			echo "I run when the sucess happens"
		}
		failure {
			echo "I run when you fail"
		}
	}
		
}
