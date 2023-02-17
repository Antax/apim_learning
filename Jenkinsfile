pipeline{

	agent any

	tools{
		maven "3.6.3"
	}

	stages{
		stage("build"){
			steps{
				git "https://github.com/Antax/apim_learning.git"
				sh "mvn clean exec:exec"
			}
		}
	}

}
