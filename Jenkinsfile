pipeline {
    agent {
        node {
            label 'AGENT-1 '
        }
    }
    stages {
        stage('Build') {
            steps {
                echo "Build stage is running"
            }
        }
        stage('Test') {
            steps {
                echo "Test stage is running"
            }
        }
        stage('Deploy') {
            steps {
                echo "Deploy stage is running"
            }
        }
    }

    //post build
    post {
        always {
            echo "Succesfully -- post_build_always"
        }
        failure {
            echo "Failed -- post_build_failure"
        }
        success {
            echo "Success -- post_build_success"
        }
    }
}