pipeline {

	 agent any
	 agent{docker {image 'node:13.8'}}
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
