pipeline {
    agent { node { label 'sonarqube'} }

    stages{
        stage('Build'){
            steps{
                echo 'Building the project...'
                sh '''
                    pwd
                    ls -la
                '''
            }
        }

    }

}

