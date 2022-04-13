pipeline {
 	agent any 
	 
		environment {
			dockerHome = tool 'dockervg'
			mavenHome = tool 'vgmaven'
			PATH = "$dockerHome/bin:$mavenHome/bin:$PATH"
		}    
		stages {
			stage("Build") {
				steps {
					echo "Build -1"
					sh 'mvn --version'
					sh 'docker version'
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
