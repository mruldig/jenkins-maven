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
#        stage('Test') { 
#            steps {
#                sh "mvn test site"
#            }
#            
#             post {
#                always {
#                    junit allowEmptyResults: true, testResults: 'target/surefire-reports/*.xml'   
#                }
#            }     
#        }

#        stage('deploy') { 
#            steps {
#                sh "mvn package"
#            }
#        }


#        stage('Build Docker image'){
#            steps {
#                sh 'docker build -t anvbhaskar/docker_jenkins_pipeline:${BUILD_NUMBER} .'
#            }
#        }
#
#        stage('Docker Login'){
#            
#            steps {
#                 withCredentials([string(credentialsId: 'DockerId', variable: 'Dockerpwd')]) {
#                    sh "docker login -u anvbhaskar -p ${Dockerpwd}"
#                }
#            }                
#        }
    }
}
