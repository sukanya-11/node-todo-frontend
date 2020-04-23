//Jenkins file only to tutorial example
pipeline {
  agent any
    
  tools {nodejs "node"}
    
  stages {
        
    stage('Cloning Git') {
      steps {
        git 'https://github.com/sukanya-11/node-todo-frontend.git'
      }
    }
        
    stage('Install dependencies') {
      steps {
        bat 'npm install'
      }
    }
     
    stage('Test') {
      steps {
         bat 'npm test'
      }
    }      
  }
}
