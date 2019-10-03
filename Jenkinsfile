pipeline {
  environment {
    def filePath= "./Deployment.yml"
     //String fileContents = new File('/Deployment.yml')
     String fileContents = new File('Deployment.yml').getText('UTF-8')
    //def fileContent = readFile.readFileString(filePath)
   }
  agent any
	  stages {
	    stage('deployment file print') {
	      steps {
		sh 'echo "dep yaml print is initialising"'
		sh 'cat $fileContents'
	        }
	      }
	    stage('find keyword in deploykent file ') {
	      steps {
		sh 'echo "dep yaml print is initialising"'
		sh 'echo $filePath'
		sh 'if grep -q quay $fileContents; then flag="True"; fi'
		sh 'echo $flag'
	      }
            } 
     }
  }
