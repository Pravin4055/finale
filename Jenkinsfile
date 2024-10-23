pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                // Clone the Git repository
                git url: 'https://github.com/your-username/your-repo.git', branch: 'main'
            }
        }

        stage('Build') {
            steps {
                echo 'Building...'
                // Add your build commands here (e.g., compiling code, running tests)
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying...'
                sh 'sh ./scripts/deploy.sh'  // Call the deploy script from your repository
            }
        }
    }

    post {
        always {
            echo 'Cleaning up...'
        }
        success {
            echo 'Job completed successfully!'
        }
        failure {
            echo 'Job failed. Please check the logs.'
        }
    }
}

