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
				sh 'sudo docker-compose down'
				sh 'sudo docker-compose up -d'
			}
		}
	}
}

