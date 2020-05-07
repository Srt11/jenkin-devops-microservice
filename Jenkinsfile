pipeline {

	 //agent any
	 agent{docker {image 'maven:3.6.3'}}
	 stages{
			stage('build'){
			  steps{
			       sh 'mvn --version'
			       echo "build"
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
