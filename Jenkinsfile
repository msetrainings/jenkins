def prepare(){
    sh "chmod +x ${WORKSPACE}/*.sh"
}

node {
    stage('Run script') {
        checkout scm
        def hello = sh(returnStdout: true, script: 'python3 ${WORKSPACE}/script.py')
        println "message: $hello"
    }
}
