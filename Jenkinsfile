pipeline {

    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/mohiturkude8237/simple-cicd-demo.git'
            }
        }

        stage('Update index.html') {
            steps {
                    sh 'cp  /var/lib/jenkins/workspace/simple-ci-cd/index.html  /var/www/html/'
                    echo 'index file updated.'
            }
        }
    }
}
