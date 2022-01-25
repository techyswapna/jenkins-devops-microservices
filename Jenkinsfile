pipeline {
	agent any
	// agent { docker { image 'node:latest'} }
	stages {
		stage('Build') {
			steps {
				// sh 'node --version'
				echo "Build"
				echo "$PATH"
				echo "BUILD_NUMBER - $env.BUILD_NUMBER"
				echo "$env.BUILD_ID"
				echo "$env.BUILD_TAG"
				echo "$env.JOB_NAME"
				}
			}
		stage('Test') {
			steps {
				echo "Test"
				}
			}
		stage('Integration Test') {
			steps {
				echo "Integration Test"
				}
			}
		} 
		post {
			always {
				echo 'Im Awesome. I run always'
			}
			success {
				echo 'I run when you are successful'
			}
			failure {
				echo 'I run when you fail'
			}
		}
}
 