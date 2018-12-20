pipeline{
	agent any
	stages{
		stage('Init'){
			steps{
				echo 'Initializing stage...'
			}
		}
		
		stage('Build'){
			steps{
				sh 'mvn clean package'
			}
			post{
				success{
					echo 'Now Arhiving...'
					archiveArtifacts artifacts: '**/*.war'
				}
			}
		}
	}
}