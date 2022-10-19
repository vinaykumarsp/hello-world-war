pipeline {
    agent { label 'slave1' }

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
                sh "cd hello-world-war"
                sh "mvn clean package"
            }
        }
        stage('Deploy') {
            steps {
                sh "cp  /home/slave1/workspace/world2/target/hello-world-war-1.0.0.war /opt/tomcat/webapps"  
            }
        }
    }
}
