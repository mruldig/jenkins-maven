pipeline {
    agent none
    stages {
        stage('Compile and Clean') { 
            agent {
                 label 'padev02.sc1.roche.com'
            }
            steps {

                sh "mvn clean compile"
            }
        }
     }
}
