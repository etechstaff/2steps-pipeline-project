pipeline {
	agent any 
	stages{
		stage('1-clonecode'){
			steps{
			checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github-credentials', url: 'https://github.com/etechstaff/2steps-pipeline-project.git']])
			}
		}
		stage('2-currently running processes'){
			steps{
				sh 'ps -ef'
			}
		}
		stage('3-Jenkins status'){
			steps{
				sh 'sudo systemctl status jenkins'
			}
		}
		
	}
}
