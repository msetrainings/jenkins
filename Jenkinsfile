node {
    stage('Load props') {
        def props = readProperties defaults: d, file: 'common.properties', text: 'other=Override'
        def url = props['url']
        def port = props['port']
        println url
        println port
    }
}
