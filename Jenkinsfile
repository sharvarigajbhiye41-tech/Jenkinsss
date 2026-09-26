pipeline {
    agent any
    envirnoment {
        APP_NAME = 'my-app'
    }
    stages {
        stage('Build') {
            steps{ 
                sh 'echo Building $APP_NAME'
            }
        }
    }
}
