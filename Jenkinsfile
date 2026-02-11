pipeline{
    agent any 
    stages{
        stage('Checkout'){
            steps{
                git url: 'https://github.com/safakhan26/jenkins-cpp-demo.git', branch:'main', credentialId:'05bb3725-45b0-45e2-9221-6edf1d9b4da7' 
            }
        }
        stage('Build'){
            steps{
                sh 'g++ test1.cpp -o main'
                }
        }
        stage('Run'){
            steps{
                sh './main'
            }
        }
    }
    
}
