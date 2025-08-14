pipeline{
    agent any
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
    }
    stages{
        stage('test'){
            steps{
                script{
                    sh '''
                     echo " hello, this is test"
                     '''
                }
            }
        }
    }
    stages{
        stege('deploy'){
            steps{
                script{
                    sh '''
                     echo " hello, this is deploy"
                     '''
                }
            }
        }
    }
}