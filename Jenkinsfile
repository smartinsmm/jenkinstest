node {
    def mvnHome = tool 'maven-3.5.2'
    tools {
            jdk "JDK"
    }
    stages{
        stage('Wich java'){
            sh 'java --version'
        }

        stage('clone repo'){
            git 'https://github.com/smartinsmm/jenkinstest.git' //git branch: 'main', url: 'https://github.com/smartinsmm/jenkinstest.git'
        }

        stage('Build project'){
            sh "'${mvnHome}/bin/mvn' -X -B -DskipTests clean package"
        }
    }
}