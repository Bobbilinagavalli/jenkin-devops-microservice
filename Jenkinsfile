pipeline {
	agent {
		docker{
			image 'valli742/hello-world-python'
		}
	}
	stages{
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
