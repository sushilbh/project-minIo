node('maven-build-agent'){
    def mvnHome = tool name: 'maven360', type: 'maven'
    echo "downloading...d.scm"
    stage('checkout'){
        git credentialsId: 'githubacc', url: 'https://github.com/sushilbh/project-minIo.git'
    }
    stage ('build'){
        echo "build the package"
        sh "${mvnHome}/mvn package -DskipTests=true"
    }
}
