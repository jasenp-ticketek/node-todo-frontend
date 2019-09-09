pipeline {
	agent any

	tools {nodejs "node"}

	stages {
		stage("Clone From Git") {
			steps {
				git "https://github.com/jasenp-ticketek/node-todo-frontend"
			}
		}

		stage("Npm Install") {
			steps {
				sh "npm i"
			}
		}

		stage("test code") {
			steps {
				sh "npm run test"
			}
		}
	}
}