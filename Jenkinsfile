node {
    stage('Run script') {
        checkout scm
        values = sh(returnStdout: true, script: '${WORKSPACE}/script.sh')
        println values
    }
}
