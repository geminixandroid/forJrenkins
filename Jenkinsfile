pipeline {
	agent any

	stages {
		stage('Checking if pipeline is enabled') {
			steps {
				if ( fileExists 'cd.enabled' ) {
					script {
						COMMIT_AUTHOR=sh(script: 'git log -1 --pretty=format:\'%an\'', returnStdout: true).trim()
						error "Pipeline was disabled by ${COMMIT_AUTHOR}"
					}
				}
				else {
					echo "Pipeline enabled"
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