pipeline{
    agent { label 'AGENT-1'}
    environment {
         PROJECT = 'EXPENSE'
         COMPONENT ='BACKEND'
    }
    options{
        disableConcurrentBuilds()
        timeout(time: 5, unit:'SECONDS')
    }
    stages{
        stage('build'){
            steps{
                script{
                    sh '''
                     echo "hello, this is build"
                     echo "Project: $PROJECT"
                     sleep 15
                     '''
                }
            }

        }
        stage('test'){
            steps{
                script{
                    sh '''
                     echo " hello, this is test"
                     '''
                }
            }
        }
        stage('deploy'){
            steps{
                script{
                    sh '''
                     echo " hello, this is deploy"
                     '''
                }
            }
        }
    }
    post {
        always{
            echo 'I will always say hello again'
        }
        failure{
            echo' I will run when pipeline is failed'
        }
        success{
            echo'I will run when pipeline is success'
        }
    }
}