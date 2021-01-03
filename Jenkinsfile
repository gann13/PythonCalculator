pipeline {
  
  stages {
     
	stage('Prepare') {
	   steps {
	   sh 'pip install -r requirements.txt
	   }
	}
	 
	stage('Build') {
	 steps {
	  sh 'chmod +x *.py'
	  sh 'python calculator.py'
	  }	  
	}
	
	stage('Test') { 
	 steps {
       sh 'pytest -v'	 
	 }
    }
	
	stage('Report') {
	  steps {
	  echo 'Test completed'
	  }
    }
 }
}
