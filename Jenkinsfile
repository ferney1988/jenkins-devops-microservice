pipeline {
	//agent any
	agent { docker { image 'node:15.7'} }
	stages {
		stage('build') {
			steps {
				sh 'node --version'
				echo "Build"
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
			echo 'Im awesome. I run always'
		}
		success {
			echo 'I run  when yo are successful'
		}
		failure {
			echo 'I run when you fail'
		}
	}
}