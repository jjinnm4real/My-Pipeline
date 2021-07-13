pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'python --version'
            }
        }
        stage ('Create HTML Report') {
            steps {
                sh "pwd"
                publishHTML([allowMissing: false, alwaysLinkToLastBuild: false, keepAll: false, reportDir: '', reportFiles: 'index.html', reportName: 'HTML Report', reportTitles: ''])
            }                
        }    
    }
}
