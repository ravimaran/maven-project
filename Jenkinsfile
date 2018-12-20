pipeline{
	agent any
	stages{
		stage('Init'){
			steps{
				echo 'Initializing stage...'
			}
		}
		
		stage('Packaging'){
			steps{
				build job: 'package'
			}
			post{
				success {
					echo 'Packaged...'
				}
			}
		}
	}
}