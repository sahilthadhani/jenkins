pipeline {
	agent any
	parameters {
  string(name: 'Greeting', defaultValue: 'Hello', description: 'How should I
greet the world?')
  }
	stages {
		stage('Build') {
			steps {
				echo 'Building.. ${param.Greeting} World!'
			}
		}
		stage('Test') {
			steps {
				echo 'Testing..'
			}
		}
		stage('Deploy') {
			try {
				steps {
					echo 'Deploying....'
				}
			} finally {
				echo 'finally....'
			}
			
		}
	}
}