
pipeline {
    agent {
        docker {
            image 'maven:3-alpine'
            args '-v $HOME/.m2:/root/.m2'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn -B'
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
