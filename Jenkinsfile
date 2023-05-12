def prepare(){
    sh "chmod +x ${WORKSPACE}/*.sh"
}

node {
    stage('Run script') {
        checkout scm
        prepare()
        def files = sh(returnStdout: true, script: '${WORKSPACE}/$scriptName')
        println "files: $files"
    }
}
