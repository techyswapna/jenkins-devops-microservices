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
				echo "BUILD_ID - $env.BUILD_ID"
				echo "BUILD_TAG - $env.BUILD_TAG"
				echo "BUILD_URL- $env.BUILD_URL"
				echo "JOB_NAME - $env.JOB_NAME"
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
 