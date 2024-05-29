// Scripted 
//declarative pipeline
pipeline {
    //agent any
		//agent {docker {image 'maven:3.6.3'} }
		agent {docker {image 'node:alpine3.19'} }
			stages {
				stage('Build'){
					steps{	
						//sh "mvn --version"
						sh 'node --version'
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
			always {	
				echo "It run always"
				}
			success {
				echo "It run on success"
				}	
			failure {
				echo "it runs on failure"	
			}	
			//unstable 
			//changed{
				//echo "it run when there is change in the status of builds"
			//}
    }
}

