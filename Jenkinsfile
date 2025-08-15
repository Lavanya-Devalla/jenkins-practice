pipeline{
    agent { label 'AGENT-1'}
    stages{
        stage('build'){
            steps{
                script{
                    sh '''
                     echo "hello, this is build"
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
        sucess{
            echo'I will run when pipeline is sucess'
        }
    }
}