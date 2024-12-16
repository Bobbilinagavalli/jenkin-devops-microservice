pipeline {
        //agent {
        //docker {
         //   image 'maven:3.6.3'
          //}
        //}
	agent any
	stages{
		stage('Build') {
			steps{
				echo "Build"
				echo "$PATH"
				echo "BUILD_NUMBER - $env.BUILD_NUMBER"
				echo "BUILD_ID - $env.BUILD_ID"
				echo "JOB_NAME - $env.JOB_NAME"
				echo "BUILD_TAG - $env.BUILD_TAG"
				echo "$env.BUILD_URL"
			}
		}
		stage('Test') {
			steps{
				echo "Test"
			}	
		}
		stage('Integration test') {
			steps{
				echo "Test"
			}
		}
	}
	post{
		always{
			echo 'I am awesome, I run always'
		}
		success{
			echo 'I run whe you are successful'
		}
		failure{
			echo 'I run when you fail'
		}
	}
		
}
