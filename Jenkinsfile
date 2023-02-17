pipeline{

	agent any

	tools{
		maven "3.6.3"
	}

	stages{
		stage("build"){
			steps{
				git config --global --unset credential.helper
				git config --system --unset credential.helper
				git "https://github.com/Antax/apim_learning.git"
				sh "mvn clean exec:java"
			}
		}
	}

}
