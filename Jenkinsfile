pipeline{
agent any

	stages{
		stage('source code'){
			steps{
				git branch: 'main', changelog: false, credentialsId: 'c2d5c505-d1a9-4995-a724-b8d65dab8007', poll: false, url: 'https://github.com/theerthak/create-react-app.git'
			}
		}
		stage('npm install'){
			steps{
				sh '''
					echo "installing dependencies"
					npm install
				'''
				}
			}
		}
	}
