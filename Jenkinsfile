node {
    stage('Run script') {
        checkout scm
        sh "chmod +x ${WORKSPACE}/script.sh"
        values = sh(returnStdout: true, script: '${WORKSPACE}/script.sh')
        println values
    }
}
