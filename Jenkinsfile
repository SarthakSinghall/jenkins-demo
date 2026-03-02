pipeline {
    agent any

    stages {

        stage('Clone Repo') {
            steps {
                git 'https://github.com/SarthakSinghall/jenkins-demo.git'
            }
        }

        stage('Deploy Website') {
            steps {
                sh '''
                docker cp index.html website:/usr/share/nginx/html/index.html
                '''
            }
        }
    }
}
