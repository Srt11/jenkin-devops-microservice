pipeline {

	 agent any
	 
	 environment{
	     dockerHome = tool 'MyDocker'
		 mavenHome = tool 'MyMaven'
		 PATH = "$dockerHome/bin:mavenHome/bin:$PATH"
	 }
	 stages{
			stage('checkout'){
			  steps{
			       sh 'mvn --version'
			       echo "build"
				   echo "$PATH"

			  }
			  }
			stage('Compile'){
			  steps{
			       sh "mvn clean compile"
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
