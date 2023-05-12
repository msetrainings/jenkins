def runScript(scriptName){
    sh "chmod +x ${WORKSPACE}/$scriptName"
    def files = sh(returnStdout: true, script: '${WORKSPACE}/$scriptName')
    println result
    return result
}

node {
    stage('Run script') {
        checkout scm
        def files = runScript('script.sh')
        println "files: $files"
    }
}
