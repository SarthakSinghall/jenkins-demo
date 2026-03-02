pipeline {
    agent any

    stages {

        stage('Show Files') {
            steps {
                sh 'ls -l'
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
