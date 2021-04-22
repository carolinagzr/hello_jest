pipeline {
   agent any

   stages {
      stage('Git') {
         steps {
          // git 'https://github.com/carolinagzr/hello_jest.git'  
         //  git 'https://github.com/AaronWatters/hello_jest.git'
           bat 'dir'
         }
      }
      stage('Build') {
         steps {
             
           
              bat 'npm install --force'
              bat 'npm install --global http-server'
            bat "npm run build" 
           
         }
      }
      stage('Test') {
         steps {
            
           bat "npm run test"
         }}
    stage('Deploy') {
         steps {
            bat "npm start" 
          
         }}
   }
}
