node {
    def mvnHome = tool 'maven-3.6.2'
    
    stage('clone repo'){
        git 'https://github.com/smartinsmm/jenkinstest.git'
    }

    stage('Build project'){
        sh "'${mvnHome}/bin/mvn' -B -DskipTests clean package"
    }
}