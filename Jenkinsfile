pipeline {
    agent any

     parameters {
        string(name: 'TARGET_PLATFORM', defaultValue: 'stmfd', description: 'Enter target platform')
        choice(name: 'BUILD_TYPE', choices: ['Debug', 'Release'], description: 'Choose build type')
        booleanParam(name: 'CLEAN_BUILD', defaultValue: true, description: 'Clean before build')
    }
    
    stages {
        stage('Prepare') {
            steps {
                echo "Target Platform: ${params.TARGET_PLATFORM}"
                echo "Build Type: ${params.BUILD_TYPE}"
                echo "Clean Build: ${params.CLEAN_BUILD}"
            }
        }
        stage('Stage 2') {
            steps {
                echo 'Running Stage 2'
                bat '''python test.py'''
            }
        }
    }
}

