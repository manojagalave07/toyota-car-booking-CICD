pipeline {
    agent any

    stages {

        stage('Clone Code') {
            steps {
                git 'https://github.com/manojagalave07/toyota-car-booking-CICD.git'
            }
        }

        stage('Build') {
            steps {
                echo "Building Toyota Booking Project"
            }
        }

        stage('Test') {
            steps {
                echo "Testing application"
            }
        }

        stage('Deploy Website') {
            steps {
                sh '''
                sudo cp -r * /var/www/html/
                '''
            }
        }
    }
}
