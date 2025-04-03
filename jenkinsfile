pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/divya3421/jenkins.git'
            }
        }
        stage('Copy HTML to Web Server') {
            steps {
                sh 'scp -o StrictHostKeyChecking=no hello.html divya3421@server:/var/www/html/'
            }
        }
    }
}
