def prepare(){
    sh "chmod +x ${WORKSPACE}/*.sh"
}

node {
    stage('Run script') {
        checkout scm
        sh "chmod +x ${WORKSPACE}/*.sh"
        def files = sh(returnStdout: true, script: '${WORKSPACE}/script.sh')
        println "files: $files"
    }
}
