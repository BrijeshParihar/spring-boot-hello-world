pipeline {
  agent any
  tools {
        maven '3.8.6' 
    }
	triggers {
        pollSCM('* * * * *')
    }

  stages {
    stage ('Clean') {
      steps {
        sh 'mvn clean'
      }
	  }
	  stage ('Compile') {
      steps {
        sh 'mvn compile'
      }
	  }
	  stage ('Test') {
      steps {
        sh 'mvn test'
      }
	  }
	  stage ('Build') {
      steps {
        sh 'mvn package'
	  }
    }
  }
}
