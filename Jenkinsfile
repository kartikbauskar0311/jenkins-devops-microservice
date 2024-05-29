// Scripted 
//declarative pipeline
pipeline {
    agent any
		stages{
			stage('Build'){
				steps{	
					echo "Build"
				}
		}
			stage('Test'){
				steps{	
					echo "Test"
				}
		}
			stage('Integration Test'){
				steps{	
					echo "Integration Test"
				}
		}
		
  }

		post {
			always{	
				echo "It run always"
				}
			success{
				echo "It run on success"
				}	
			failure{
				echo "it runs on failure"	
			}	
			//unstable 
			//changed
    }
}

