pipeline {
  agent any
  stages{
    stage ('Build') {
      steps{
        echo "Building Project"
        sh './mvnw package'
      }
    }
    stage ('Archive') {
      steps{
        echo "Archiving Project"
        archiveArtifacts artifacts: '**/*.jar', followSymlinks: false
      }
    }
    stage ('Build Docker Image') {
      steps{
        echo "Building Docker Image"
      }
    }
    stage ('Push Docker Image') {
      steps{
        echo "Pushing Docker Image"
      }
    }
    stage ('Deploy to Dev') {
      steps{
        echo "Deploying to Dev Environment"
      }
    }
  }
}
