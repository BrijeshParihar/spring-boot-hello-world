pipeline {
  agent any
  tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven 'Maven 3.8.7' 
    }
  stages {
    stage ('Build') {
      steps {
        sh 'mvn clean install -DskipTests'
      }
    }
  }
}
