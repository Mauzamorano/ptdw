pipeline{
	agent any
	stages{
		stage('Initial setup'){
			steps{
				sh 'echo starting'
			}
		}

		stage('Checking Docker'){
			steps{
				sh 'sudo docker ps'
			}
		}
		
		stage ('Prueba Docker'){
			steps{
			 sh "docker-compose -f docker-compose.integration.yml up --force-recreate --abort-on-container-exit"
			}
		}
	}
}

