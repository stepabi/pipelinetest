pipeline {
    agent any
    stages {
        stage('Test') {
            steps {
                sh 'echo "It is working"'
                sh '''
                    echo "List local file"
                    ls -lah
                '''
            }
        }
        stage('Build'){
            steps{
                sh 'docker build -f Dockerfile -t testing .'
            }
        }
    }
}