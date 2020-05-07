pipeline {

	 agent any
	 //agent{docker {image 'node:13.8'}}
	 environment{
	     dockerHome = tool 'myDocker'
		 mavenHome = tools 'myMaven'
		 PATH = "$dockerHome/bin:mavenHome/bin:$PATH"
	 }
	 stages{
			stage('build'){
			  steps{
			       //sh 'node --version'
			       echo "build"
				   echo "$PATH"

			  }
			  }
			stage('test'){
			  steps{
			       echo "test"
			  }
			  }
			stage('Integration test'){
			  steps{
			       echo "Integration test"
			  }
			  }
		 }
	 
}
