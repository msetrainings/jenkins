node {
    stage('Run script') {
        checkout scm 
        def script = readFile('script.sh')
        script.execute()
    }
}
