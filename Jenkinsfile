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
		sh 'echo $filePath'
		sh 'if grep quay $filePath; then flag="True"; fi'
		sh 'echo $flag'
	      }
            } 
     }
  }
