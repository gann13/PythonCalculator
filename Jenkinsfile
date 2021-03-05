pipeline {

	agent any

	stages {

		stage('Build') {
			steps {
				sh 'docker build . -t kp-calculator:1.0'
			}
		
		stage('Test') {
			steps {
				sh 'docker run kp-calculator'
			}

		stage('Deploy') {
			steps {
				sh 'docker push'
			}
		} 
		}

		}



	}

}