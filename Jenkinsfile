pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                echo 'Cloning Source Code'
            }
        }

        stage('Build') {
            steps {
                echo 'Building Application'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                sudo cp -r * /var/www/html/
                sudo systemctl restart httpd
                '''
            }
        }
    }
}
