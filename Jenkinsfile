pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'Building'
          }
        }

        stage('ParallelBuild') {
          steps {
            echo 'Parallel building'
          }
        }

      }
    }

    stage('test') {
      steps {
        echo 'Testing'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying'
      }
    }

  }
}