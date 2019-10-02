pipeline {
  environment {
    def filePath= "./Deployment.yml"
    //def fileContent = readFile.readFileString(filePath)
   }
  agent any
	  stages {
	    stage('deployment file print') {
	      steps {
		sh 'echo "dep yaml print is initialising"'
		sh 'cat Deployment.yml'
	        }
	      }
	    stage('find keyword in deploykent file ') {
	      steps {
		sh 'echo "dep yaml print is initialising"'
		sh 'if grep quay $filepath; then flag = True; fi'
	      }
            } 
     }
  }
