pipeline {
	agent {
		docker {
			image "maven:3.6.3"
		}
	}
	stages {
		stage('Build') {
			steps {
				sh "mv --version"
				echo "Build"
			}
		}
		stage('Test') {
			steps {
				echo "Test"
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
