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
				echo 'building...'
				build job: 'jenkinsfile-package'
			}
			post{
				success {
					echo 'Built successfully...'
				}
			}
		}
	}
}