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
        stage ('Create HTML Folder') {
            steps {
                publishHTML([allowMissing: false, alwaysLinkToLastBuild: false, keepAll: false, reportDir: '', reportFiles: 'index.html', reportName: 'HTML Report', reportTitles: ''])
            }                
        }    
    }
}
