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
			 sh "docker-compose -f /backup/d4a/docker-compose.yml up --force-recreate --abort-on-container-exit"
			}
		}
	}
}

