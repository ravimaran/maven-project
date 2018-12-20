pipeline{
	agent any
	tools{
		maven 'localMaven'
	}
	
	stages{
		stage('Init'){
			steps{
				echo 'Initializing stage...'
			}
		}
		
		stage('Build'){
			steps{
				echo 'building...'
				sh 'mvn clean package'
			}
			post{
				success {
					echo 'Built successfully...'
				}
			}
		}
	}
}