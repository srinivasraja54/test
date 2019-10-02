pipeline {
  environment {
    file_name = "Deployment.yml"
   }
  agent any
	  stages {
	    stage('Dockerfile print') {
	      steps {
		sh 'echo "dockerfile print is initialising"'
		sh 'cat Dockerfile'
	        }
	      }
     }
   }
