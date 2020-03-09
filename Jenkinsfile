pipeline {
    agent any
    tools {
      jdk "my_jdk8"  
      maven "my_maven"
    }
    stages {
        stage (build) {
            steps {
                sh "mv compile"
                echo "This does testing...!"
            }
        }
        
        stage (package) {
            steps {
                sh "mvn package"
                echo "This does packaging"
            }
        }
    }
}
