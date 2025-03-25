pipeline {
    agent { node {label 'sonarcli'} }

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
                sh 'whoami'
                sh 'ls'
                echo 'Building the project...'
                sh 'npm install'
            }
        }
        stage('scan'){
            steps{
                echo 'Building the project...'
                sh '''
                    ls -la
                    pwd
                    echo "Hello "
                    whoami
                    ls -la
                '''
            }
        }
        stage('sonarscan'){
            steps{
                sh 'sonar-scanner'
            }
        }

    }
    post {
        always {
            cleanWs()  // Cleans the workspace after execution
            echo 'Workspace cleaned up!'
        }
    }
}


