pipeline {
    agent any

    tools{
        jdk 'my_jdk8'
        maven 'my_maven'
    }
    stages {
    stage('build') {
        steps{
            echo "This is the build step"
            sh 'mvn compile'
        }

    }
    stage('test') {
        steps{
            echo "This is testing"
            sh 'mvn test'
        }
    }
    stage('package') {
        steps{

            echo "packaging in pipeline"
            sh 'mvn package'
        }
    }
}
}
