pipeline {
    agent any
    stages {
        stage('cloning my git repo') {
            steps {
                git branch: 'master', url: 'https://github.com/surnalliuvinod/jens.git'
            }
        }
        stage('build') {
            steps {
                sh "mvn install"
				
            }
        }
        stage('deploy') {
            steps {
                sh "ansible --version"
            }
        }
    }
}
