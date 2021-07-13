pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'python --version'
            }
        }
        stage('Create new folder') {
            steps {
                sh "mkdir html_report"
            }    
        }
    }
}
