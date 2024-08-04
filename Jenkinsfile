pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                // Lệnh để xây dựng dự án, ví dụ: mvn clean install
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                // Lệnh để kiểm tra dự án, ví dụ: mvn test
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Lệnh để triển khai dự án, ví dụ: scp target/*.jar user@server:/path/to/deploy/
            }
        }
    }
    post {
        always {
            echo 'This will always run'
        }
        success {
            echo 'This will run only if successful'
        }
        failure {
            echo 'This will run only if failed'
        }
    }
}
