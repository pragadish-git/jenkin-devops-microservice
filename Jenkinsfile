pipeline {
	agent {
		docker {
			image 'maven:3.6.3'
		}
	}
	stages {
		stage('Build') {
			steps {
				sh 'mvn --version'
				echo "Build"
			}
		}
		stage('Test') {
			steps {
				echo "Test"
			}
		}
		stage('Deploy') {
			steps {
				echo "Deployed"
			}
		}
	}

	post {
		always {
			echo "Always"
		}
		success {
			echo "successfull"
		}
		failure {
			echo "failure"
		}
	}
}
