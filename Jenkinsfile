pipeline {
    agent none
    stages {
        //START OF THE BUILD STAGE 
        stage('Build'){
            agent{label 'BDP'}
            steps{
                script{
                    sh "echo 'Build stage triggered'"
                }
            }
        }
        //END OF BUILD STAGE
        //START OF THE DEVL STAGE 
        stage('Devl'){
            agent{label 'BDP'}
            steps{
                script{
                    sh "echo 'Devl Deploy stage triggered'"
                }
                checkpoint ""
            }
        }  
        //END OF THE DEVL STAGE  
        //START OF THE TEST STAGE 
        stage('TEST'){
            agent{label 'BDP'}
            steps{
                script{
                    sh "echo 'TEST Deploy stage triggered'"
                }
                checkpoint ""
            }
        }  
        //END OF THE TEST STAGE  
        //START OF THE ACPT STAGE
        stage('ACPT'){
            agent{label 'BDP'}
            steps{
                script{
                    sh "echo 'ACPT Deploy stage triggered'"
                }
                checkpoint ""
            }
        }  
        //END OF THE ACPT STAGE  
        //START OF THE PROD STAGE
        stage('PROD'){
            agent{label 'BDP'}
            steps{
                script{
                    sh "echo 'PROD Deploy stage triggered'"
                }
                checkpoint ""
            }
        }  
        //END OF THE PROD STAGE  
    }
}
