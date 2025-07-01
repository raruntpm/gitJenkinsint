pipeline {
    agent {
        label 'stmfd-build-server'
    }
    stages {
        stage('Check Agent') {
            steps {
                echo 'Running on stmfd-build-server...'
                sh '''
                    echo "Agent is connected!"
                    echo "Hostname: $(hostname)"
                    echo "User: $(whoami)"
                    echo "Current Directory: $(pwd)"
                    echo "Disk Space:"
                    df -h
                '''
            }
        }
    }
}
