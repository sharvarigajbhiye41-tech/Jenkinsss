pipeline {
    agent any
    parameters {
        choice(name: 'ENVIRONMENT' , choices: ['staging','production'], description:'Target')
    }
    stages {
        stage('Approve') {
         steps {
             input message: 'Deploy to production?'
            }
        }
    }
    post {
       success {
         echo 'Pipeline succeeded'
       }
       failure {
           echo 'Pipeline failed'
       }
}
