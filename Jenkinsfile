pipeline {
    agent { label "build" }
    stages {
         stage("checkout"){
             steps {
                checkout scm
             }
         }
         stage("build") {
             steps {
                 sh "sudo docker build -t sampleapp ."
             }
         }
         stage("run") {
             steps {
                 sh "sudo docker run -d -p 5000:5000 --name sampleapp sampleapp"
             }
         }
     }
}
