pipeline {
    agent any
    environment {
        PATH = '/bin:$PATH'
    }
    
    stages {
        stage ("git") {
            steps {
                git branch: 'main', url: 'https://github.com/Anil14433/pet_shop.git'
            }
        }
        stage("build") {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}
