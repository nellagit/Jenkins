pipeline{

  agent any
  stages{
      stage('build step') {
          steps {
              script {
                  def customImage = docker.build("my-image:${env.BUILD_ID}", "-f Dockerfile .")       
              }
          }
      }
  }  
}