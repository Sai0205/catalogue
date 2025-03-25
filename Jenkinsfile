pipeline {
    agent { node {label 'sonarscan'} }
    stages{
        stage('Build'){
            steps{
                echo 'Building the project...'
                sh '''
                    pwd
                    ls
                '''
            }
        }

    }

}

