node {
    stage('Load props') {
        Properties properties = new Properties()
        File propertiesFile = new File('common.properties')
        propertiesFile.withInputStream {
            properties.load(it)
        }
        def runtimeString = 'a'
        assert properties."$runtimeString" == '1'
        assert properties.b == '2'
    }
}
