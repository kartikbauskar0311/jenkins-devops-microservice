// Scripted 
//declarative pipeline
pipeline {
    //agent any
		//agent {docker {image 'maven:3.6.3'} }
		//agent {docker {image 'node:alpine3.19'} }
			
			stages {
				stage('Build'){
					steps {	
						//sh "mvn --version"
						//sh 'node --version'
						echo "Build"
						echo "PATH - $PATH"
						echo "BUILD_ID - $env.BUILD_ID"
						echo "BUILD_NUMBER - $env.BUILD_NUMBER"
						echo "JOB_NAME - $env.JOB_NAME"
						echo "BUILD_TAG - $env.BUILD_TAG"
						echo "BUILD_URL - $env.BUILD_URL"
					}
			}
				stage('Test'){
					steps {	
						echo "Test"
					}
			}
				stage('Integration Test'){
					steps {	
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

