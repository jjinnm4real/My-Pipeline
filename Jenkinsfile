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
                sh "pwd"
            }    
        }
        stage ('Build HTML Report') {
            steps {
                publishHTML([allowMissing: false, alwaysLinkToLastBuild: false, keepAll: false, reportDir: '/html_report', reportFiles: 'index.html', reportName: 'HTML Report', reportTitles: ''])
            }                
        }    
    }
}
