pipeline {

	 agent any
	 //agent{docker {image 'node:13.8'}}
	 environment{
	     dockerHome = tool 'MyDocker'
		 mavenHome = tools 'MyMaven'
		 PATH = "$dockerHome/bin:mavenHome/bin:$PATH"
	 }
	 stages{
			stage('checkout'){
			  steps{
			       //sh 'node --version'
			       echo "build"
				   echo "$PATH"

			  }
			  }
			stage('Compile'){
			  steps{
			       sh "mvn clean complie"
			  }
			  }
			stage(' test'){
			  steps{
			       sh "mvn test"
			  }
			  }
			stage(' Integration test'){
			  steps{
			       sh "mvn failsafe:integration-test failsafe:verify"
			  }
			  }
		 }
	 
}
