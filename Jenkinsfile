pipeline {
    agent any
    
    tools {
        jdk "jdk17-0-5"
    }
    
    stages {
        stage('Build') {
            steps {
                git branch: 'master', url: 'https://github.com/BPLJLR/demo-retourdevacances'
                sh "chmod +x ./gradlew"
                sh "./gradlew build"
            }
        }
        stage('Coucou') {
            steps {
                sh "echo 'coucou'"
            }
        }
    }
}
