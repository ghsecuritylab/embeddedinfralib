ccola_component(network_test gmock_test)

    ccola_sources(
        TestCertificatesMbedTls.cpp
        TestConnectionMbedTls.cpp
        TestConnectionSerial.cpp
        TestDnsResolver.cpp
        TestExclusiveConnection.cpp
        TestHttpClient.cpp
        TestHttpClientAuthentication.cpp
        TestHttpClientBasic.cpp
        TestHttpClientJson.cpp
        TestHttpServer.cpp
        TestLlmnrResponder.cpp
        TestMqttClient.cpp
        TestNameResolverCache.cpp
        TestSerialServer.cpp
        TestSingleConnectionListener.cpp
        TestSntpClient.cpp
        TestWebSocketClient.cpp
        TestWebSocketClientConnectionObserver.cpp
        TestWebSocketIntegration.cpp
        TestWebSocketServerConnectionObserver.cpp
    )

    ccola_dependencies(
        network
        network_test_doubles
        infra.timer_test_helper
        infra.util_test_helper
        hal.generic
        hal.test_doubles
        hal.synchronous_test_doubles
        services.util
    )

ccola_end_component()
