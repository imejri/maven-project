pipeline {
    agent any
    triggers {
         pollSCM('* * * * *')
    stages{
        stage('Build'){
            steps {
                sh 'echo build stage'
            }
            post {
                success {
                    echo 'Now Archiving...'
                    echo 'archive artifact'
                }
                failure { echo 'error on the build steps !!!'}
            }
        }
    }
}