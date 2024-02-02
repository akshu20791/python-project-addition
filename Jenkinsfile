pipeline {
    agent any
    stages{
        stage('git cloned'){
            steps{
                git url:'https://github.com/akshu20791/python-project-addition', branch: "master"
              
            }
        }
    stage('Build the project') {
            steps {
               sh "mvn sudo apt-get update"
               sh "mvn sudo apt-get upgrade"
               sh "mvn sudo apt-get install -y build-essential"
              sudo apt-get install -y libbz2-dev
            }
        }
    }
  
