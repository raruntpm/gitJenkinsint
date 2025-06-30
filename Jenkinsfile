pipeline {
    agent any

    stages {
        stage('Stage 1') {
            steps {
                echo 'Running Stage 1'
            }
        }
        stage('Stage 2') {
            steps {
                echo 'Running Stage 2'
                python3 test.py
            }
        }
    }
}

