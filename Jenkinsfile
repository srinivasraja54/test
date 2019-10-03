pipeline {
  environment {
    def filePath= "./Deployment.yml"
    def version = readFile "Deployment.yml"
   }
  agent any
	  stages {
	    stage('deployment file print') {
	      steps {
		sh 'echo "dep yaml print is initialising"'
		sh 'cat $version'
		if (version.contains("quay"))  {
		      	print "contains"
		 } else {
		    print "doesnt contains"
	         }
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
