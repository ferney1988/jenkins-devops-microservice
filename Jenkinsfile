pipeline {
	//agent any
	agent { docker { image 'node:alpine3.10'} }
	stages {
		stage('build') {
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