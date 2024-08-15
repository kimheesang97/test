pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Git 리포지토리에서 소스 코드를 체크아웃
                git 'https://github.com/kimheesang97/test.git'
            }
        }
        stage('Build') {
            steps {
                // 빌드 명령어 실행 (예: 컴파일, 패키징)
                sh 'echo "Building the project..."'
                // 실제 빌드 명령어를 여기에 추가하세요
            }
        }
        stage('Test') {
            steps {
                // 테스트 명령어 실행
                sh 'echo "Running tests..."'
                // 실제 테스트 명령어를 여기에 추가하세요
            }
        }
        stage('Deploy') {
            steps {
                // 배포 명령어 실행 (예: 서버에 배포)
                sh 'echo "Deploying the project..."'
                // 실제 배포 명령어를 여기에 추가하세요
            }
        }
    }

    post {
        always {
            // 빌드 완료 후 실행되는 작업
            echo 'Pipeline finished.'
        }
        success {
            // 빌드 성공 시 실행되는 작업
            echo 'Build succeeded!'
        }
        failure {
            // 빌드 실패 시 실행되는 작업
            echo 'Build failed.'
        }
    }
}

