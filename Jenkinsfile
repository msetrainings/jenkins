node {
    stage('Load props') {
        def d = [test: 'Default', something: 'Default', other: 'Default']
        def props = readProperties defaults: d, file: 'common.properties', text: 'other=Override'
        def url = props['url']
        def port = props['port']
        println url
        println port
    }
}
