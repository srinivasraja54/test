pipeline {
  environment {
    def filePath= "./Deployment.yml"
    def version = readFile "Deployment.yml"
    def lines = new File('Deployment.yml').readLines()
    def result = lines.findAll { it.contains('quay') }
    //println result*.toString()
   }
  agent any
	  stages {
	    stage('deployment file print') {
	      steps {
		sh 'echo "dep yaml print is initialising"'
		sh 'cat $result'
	      }
	      }
	    //stage('find keyword in deploykent file ') {
	     // steps {
		//sh 'echo "dep yaml print is initialising"'
		//sh 'echo $filePath'
		//sh 'if grep -q quay $version; then flag="True"; fi'
		//sh 'echo $flag'
	      //}
            //} 
     }
  }
