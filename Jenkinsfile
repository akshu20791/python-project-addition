pipeline {
    agent any
    stages {
        stage('git checkout') {
            steps {
                git url: 'https://github.com/akshu20791/python-project-addition', branch: 'main'
            }
        }
        stage('Build the project') {
            steps {
                sh "sudo apt-get update"
                sh "sudo apt-get install -y build-essential"
                sh "mvn clean install" // assuming Maven is already installed
            }
        }
    }
}
