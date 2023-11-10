pipeline {
    agent any

    stages {
        stage ('CloneFromGithub') {
            steps {
                script{
                    git branch: 'main', url: 'https://github.com/OlayinkaBo/jenkins-test.git'
                    sh 'ls'
                }
            }
        }
        stage ('Build') {
            steps{
                script{
                    sh 'echo "Building....."'
                }
            }
        }
         stage ('Docker') {
            steps{
                script{
                    sh 'docker --version'
                }
            }
        }
        stage ('Deploy') {
            steps {
                script{
                    sh 'echo "Deployment successful"'
                }
            }
        }
    }
}

