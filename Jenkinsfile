pipeline {
   agent any

   tools {
      // Install the Maven version configured as "M3" and add it to the path.
      maven "M3"
   }

   stages {
      stage('Build') {
         steps {
            // Get some code from a GitHub repository
            dir('cadvisor1') {
                git 'https://github.com/google/cadvisor.git'
                sh "pwd"
            }

            // Run Maven on a Unix agent.
            sh "echo putanja trenutna je"
            sh "pwd"
            sh "ls -la"
            
            dir('cadvisor2') {
                git 'https://github.com/google/cadvisor.git'
                sh "pwd"
            }

           sh "echo putanja trenutna je"
            sh "pwd"
            sh "ls -la"
         }
      }
      stage ('Test') {
          steps {
            sh "ls -la"
            sh "pwd"     
          }
         
      }
   }
}

