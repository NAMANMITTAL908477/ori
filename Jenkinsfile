
pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/NAMANMITTAL908477/ori.git'
            }
        }
        stage('Update ori.html') {
            steps {
                // Replace the content of ori.html with your desired content
                sh 'sed -i "s/old_content/new_content/" ori.html'
            }
        }
        stage('Commit and Push') {
            steps {
                sh 'git add ori.html'
                sh 'git commit -m "Updated ori.html"'
                sh 'git push origin main'
            }
        }
    }
}
