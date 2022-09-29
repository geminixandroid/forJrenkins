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
				script {
					def author = sh(returnStdout: true, script: "git log -1 --pretty=format:'%an'").trim()
					echo "$author"
					error "The build number is ${author}"
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