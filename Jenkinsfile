pipeline{

    agent any
    stages{
        stage('build step') {
            steps {
                script {
                    def customImage = docker.build("my-image:${env.BUILD_ID}", "-f Dockerfile .") {

                    }      
                }
            }
        }
        stage('run step') {
            steps {
                script {
                    docker.image("my-image:${env.BUILD_ID}").withRun('-p 80:80') {
                        
                    }
                }
            }
        }
    }  
}