properties([pipelineTriggers([githubPush()])])
node('master'){
    //def mvnHome = tool name: 'maven360', type: 'maven'
    echo "downloading...scm"
    echo "Testing smee...!!"
    stage('checkout'){
        git credentialsId: 'githubacc', url: 'https://github.com/sushilbh/project-minIo.git'
    }
    stage ('build'){
        echo "build the package"
        //sh "${mvnHome}/mvn package -DskipTests=true"
        sh "ls -latr"
        sh "cat Jenkinsfile"
    }
}
