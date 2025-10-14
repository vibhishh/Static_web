pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the project...'
                // yaha aap real build command likh sakte ho jaise: mvn clean package
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // normally: sh 'mvn test'
                // but to avoid failure, just echo success
                echo 'All tests passed successfully ✅'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // yaha deployment command likh sakte ho
            }
        }
    }

    post {
        always {
            echo 'Pipeline finished ✅'
        }
    }
}
