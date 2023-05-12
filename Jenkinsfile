def runScript(scriptName){
    sh "chmod +x $scriptName"
    def result = sh(returnStdout: true, script: '${scriptName}')
    println result
    return result
}

node {
    stage('Run script') {
        checkout scm
        def files = runScript('${WORKSPACE}/script.sh')
        println "files: $files"
    }
}
