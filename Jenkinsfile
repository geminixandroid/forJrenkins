pipeline {
	agent any

	stages {
		stage('Check lock file exists') {
			when {
				expression {
					true
				}
			}
			steps {
				echo 
				script {
					CHANGE_AUTHOR = sh(script: 'echo $CHANGE_AUTHOR', ,returnStdout: true)
					error CHANGE_AUTHOR
				}
			}
		}
		stage('Build tools') {
			steps {
				echo 'Building tools..'
			}
		}
		stage('Stage 3') {
			steps {
				echo 'Stage 3..'
			}
		}
		stage('Stage 4') {
			steps {
				echo 'Stage 4..'
			}
		}
		stage('Stage 5') {
			steps {
				echo 'Stage 5..'
			}
		}
		stage('Stage 6') {
			steps {
				echo 'Stage 6..'
			}
		}
		stage('Stage 7') {
			steps {
				echo 'Stage 7..'
			}
		}
		
	}
}