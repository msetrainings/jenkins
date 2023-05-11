node {
    stage('Load props') {
        def props = readProperties file: 'common.properties'
        def url = props['url']
        def port = props['port']
        println url
        println port
    }
}
