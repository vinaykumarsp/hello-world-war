pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                sh "pwd"
                sh "rm -rf hello-world-war"
                sh "git clone https://github.com/vinaykumarsp/hello-world-war.git"
            }
        }
        stage('build') {
            steps {
                sh "ls"
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
