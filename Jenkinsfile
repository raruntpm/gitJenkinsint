pipeline {
  agent any
  stages {
    stage('Example Build') {
      steps {
        echo 'echo Hello World'
      }
    }
    stage('Example Deploy') {
      when {
        branch 'main'
      }
      steps {
        echo 'echo Deploying'
      }
    }
  }
}
