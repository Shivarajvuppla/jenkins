pipeline {
	// agent any
	agent { docker { image 'in28min/hello-world-java:0.0.2.RELEASE' } }
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
