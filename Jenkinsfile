pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: '67b08383-6c2e-4145-a503-5763ec1b6d4d', url: 'https://github.com/Ayushaps1/DevopsAssesment.git']]])
            }
        }
        stage('Build'){
            steps{
                echo'The job has been build.'
            }
        }
        stage('Test'){
            steps{
                echo'The job has been tested.'
            }
        }
        stage('Deploy'){
            steps{
                echo'The job has been deployed.'
            }
        }
    }
}
