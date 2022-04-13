pipeline {
 	agent { docker { image 'node:13.8' } }  
		stages {
			stage("Build") {
				steps {
					echo "Build -1"
				}
			}
			stage("Test") {
				steps {
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
