pipeline {
    agent any

    stages {
        stage('Fetch code') {
            steps {
                git branch: 'main', url: 'https://github.com/mdshaibazkhan/pipeline-demo.git'
            }
        }
        stage('Install apache') {
            steps {
                sh 'sudo apt install apache2 -y'
            }
        }
        stage('Deploy code') {
            steps {
                sh 'sudo cp -R */var/www/html/'
            }
        }
    }
}
