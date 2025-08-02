pipeline{
    agent any


    stages{
        stage('Cloning Github repo to Jenkins'){
            steps{
                script{
                    echo 'Cloning Github repo to Jenkins....................'
                    checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github-token', url: 'https://github.com/udaykumar-007/udemy_mlops_1_hotel_reservations.git']])
                }
            }
        }
    }
}