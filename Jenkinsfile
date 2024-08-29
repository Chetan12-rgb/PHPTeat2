pipeline {
    agent any

    stages {
        stage('fetch'){
            steps{
                git branch: 'main', url: 'https://github.com/Chetan12-rgb/PHPTeat2.git'
            }
        }
        stage('check'){
            steps{
                sh 'ls'
            }
        }
        stage('conatiner'){
            steps{
                sh 'docker build -t myphp .'
                sh 'docker run --name my_php6 -d -p 80:80 myphp '
                
            }
        }
    }
}
