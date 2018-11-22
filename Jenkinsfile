pipeline {
    agent any
    stages {
         stage("checkout"){
             steps {
                checkout scm
             }
         }
         stage("result") {
             steps {
                 echo "Build successful"
             }
         }
     }
}
