pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'python --version'
            }
        }
        state('Create new folder') {
            steps {
                sh "mkdir html_report"
            }    
        }
    }
}
