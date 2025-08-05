pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Kodlar alınıyor...'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'pip install -r requirements.txt || true'
            }
        }

        stage('Run Tests') {
            steps {
                echo 'Testler çalıştırılıyor...'
                sh 'python3 -m unittest test_app.py'
            }
        }
    }
}
