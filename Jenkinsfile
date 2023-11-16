pipeline {
	options {
    buildDiscarder(logRotator(numToKeepStr: '10', artifactNumToKeepStr: '10'))
	}
    /* agent { docker { image 'node:20.9.0-alpine3.18' } } */
    agent "Ansible_Agent"
    stages {
        stage('Clean workspace') {
            steps {
                cleanWs()
            }
        }
    }
}

