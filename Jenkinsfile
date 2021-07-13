pipeline {
    agent { docker { image 'python:3.5.1' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
            }
        }
        stage ('Generate HTML Report') {
            steps {
                publishHTML (target : [allowMissing: false,
                    alwaysLinkToLastBuild: true,
                    keepAll: true,
                    reportDir: '',
                    reportFiles: 'myreport.html',
                    reportName: 'My Reports',
                    reportTitles: 'The Report'])
                }    
            }    
        }    
    }
}
