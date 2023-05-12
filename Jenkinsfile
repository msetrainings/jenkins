def runScript(scriptName){
    sh "chmod +x $scriptName"
    def result = sh(returnStdout: true, script: '${scriptName}')
    println result
    return result
}

node {
    stage('Run script') {
        checkout scm
        sh "chmod +x ${WORKSPACE}/script.sh"
        def files = sh(returnStdout: true, script: '${WORKSPACE}/script.sh')
        println "files: $files"
    }
}
