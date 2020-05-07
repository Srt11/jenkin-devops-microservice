pipeline {

	 agent any
	 stages{
			stage('build'){
			  steps{
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
	   post{
		  always{
		  echo ' im awesome'
		  }
		  sucess{
		  echo "sucess"
		  }
		  failure{
		  echo "failure"}
		  }
}
