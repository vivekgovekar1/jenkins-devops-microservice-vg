pipeline {
	# agent any
	agent { docker {image 'maven:3.6.3'}}  
		stages {
			stage("Build") {
				steps {
					echo "Build -1"
				}
			}
			stage("Test") {
				steps {
					sh 'mvn --version'
					echo "Test -1"
				}
			}		
			stage("Intgration Test") {
				steps {
					echo "Intgration Test -1"
				}
			}
		}
		post{
			always{
				echo ">> In Post Always"
			}
			success{
				echo ">> In Post success"
			}
			failure {
				echo ">> In Post failure"

			}
	   }
}  
