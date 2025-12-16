 pipeline {
    agent {
        docker {
            image 'python:3.14'
        }
    }

    stages {
        stage('build') {
            steps {
                git branch: 'main', url: 'https://github.com/axelinho75/Processus_text.git'
                
                sh "python3 main.py"
            }
        }
    }
}
