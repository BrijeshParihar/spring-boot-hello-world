pipeline {
  agent any
  tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven '3.8.6' 
    }
  stages {
    stage ('Build') {
      steps {
        sh 'mvn clean install -DskipTests'
      }
    }
  }
}
