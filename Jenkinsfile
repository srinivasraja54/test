pipeline {
  environment {
    def filePath= "./Deployment.yml"
    def version = readFile "Deployment.yml"
    def lines = new File('Deployment.yml').readLines()
    def result1 = new File('Deployment.yml').readLines().grep(~/[q][u][a][y]/)
    def result = lines.findAll { it.contains('quay') }
    println (result1)
    println (result)
   }
  agent any
  stages {
	    stage('deployment file print') {
	      steps {
		sh 'echo "dep yaml print is initialising"'
		sh 'cat $result'
	      }
	  }
     }
}
