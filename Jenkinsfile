pipeline {
  environment {
    def filePath= "./Deployment.yml"
    env.WORKSPACE = pwd()
    def version = readFile "${env.WORKSPACE}/Deployment.yml"
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
		sh 'if grep -q quay $version; then flag="True"; fi'
		sh 'echo $flag'
	      }
            } 
     }
  }
