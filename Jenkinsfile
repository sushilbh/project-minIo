node('maven-build-agent'){
    def mvnHome = tool name: 'maven360', type: 'maven'
    echo "downloading scm"
    stage('checkout'){
        git credentialsId: 'githubacc', url: 'https://github.com/sushilbh/project-minIo.git'
    }
}
