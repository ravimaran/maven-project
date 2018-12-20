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
				echo 'Creating package'
				sh 'mvn clean package'
			}
		}
	}
}