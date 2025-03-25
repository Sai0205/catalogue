pipeline {
    agent { node { label 'sonarqube'} }

     options {
        skipDefaultCheckout()  // Disables automatic git checkout
    }

    stages{
        stage('Build'){
            steps{
                echo 'Building the project...'
                sh '''
                    pwd
                    ls -la
                    echo "hi"
                '''
            }
        }

    }

}

