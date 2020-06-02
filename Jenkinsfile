pipeline {
	agent any
	stages {
	   stage('Build') {
		  steps{
		    echo "Build"
		  }
	    }
	    stage('Test') {
		 steps{
		   echo "Test"
		 }
	    }
	}
	post{
		success{
			echo "sucess build"
		}
		failure{
			echo "build falied"
		}
		always{
			echo "always run Abdur"
		}
	}
}
