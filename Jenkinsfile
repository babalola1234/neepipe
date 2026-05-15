pipeline {
    agent {
        label 'slave'
    }
    stages {
        stage('get the code from github') {
            steps {
				//Check out your source code repository
                checkout scm
            }
        }
		stage('check web page') {
            steps {
				sh 'touch index.html'
				sh 'echo welcome to my page > index.html'
				sh 'cat index.html'
				sh 'man date > date.txt'
            }
        }
		stage('make redht user') {
            steps {
				sh 'sudo useradd redhat'
		
            }
        }
    }
}
