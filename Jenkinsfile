pipeline {
    agent any

    triggers {
        pollSCM('* * * * *') // Poll SCM every minute
    }

    stages {
        stage('Build') {
            when {
                branch 'develop'
            }
            steps {
                echo 'Building project on develop branch'
            }
        }
    }
}
