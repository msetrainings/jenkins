node {
    stage('Run script') {
        checkout scm
        values = sh(returnStdout: true, script: 'script.sh')
        println values
    }
}
