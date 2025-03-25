pipeline {
    agent { node {label 'sonarscan'} }

    stage( sonarscan){
        steps{
            sh "echo 'Building the project..."
        }
    }
}

