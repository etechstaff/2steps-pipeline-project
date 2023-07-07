pipeline {
	agent any 
	stages{
		stage('1-clonecode'){
			steps{
			sh 'echo "welcome to jenkins demo"'
			}
		}
		stage('2-currently running processes'){
			steps{
				sh 'ps -ef'
			}
		}
		stage('3-Jenkins status'){
			steps{
				sh 'sudo systemctl status Jenkins'
			}
		}
		
	}
}