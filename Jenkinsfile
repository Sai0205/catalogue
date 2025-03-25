pipeline {
    agent { node {label 'sonarqube'}}

    //  options {
    //     skipDefaultCheckout()  // Disables automatic git checkout
    // }

    stages{
        // stage('Checkout'){
        //     steps{
        //         echo 'Checking out the code...'
        //         git branch: 'main', url: 'https://github.com/saikiranpi/Mastering-Docker.git'
        //     }
        // }
        stage('Build'){
            steps{
                echo 'Building the project...'
                sh 'npm install'
            }
        }
        stage('Build'){
            steps{
                echo 'Building the project...'
                sh '''
                    ls -la
                    pwd
                '''
            }
        }

    }
}


