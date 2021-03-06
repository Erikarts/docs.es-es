# [Ejemplos de Windows Communication Foundation](index.md)
## [Instrucciones de instalación](set-up-instructions.md)
### [Procedimiento de instalación única para los ejemplos de Windows Communication Foundation](one-time-setup-procedure-for-the-wcf-samples.md)
#### [Instrucciones de firewall](firewall-instructions.md)
#### [Instrucciones de hospedaje de Internet Information Services](internet-information-service-hosting-instructions.md)
#### [Instrucciones de instalación del certificado de servidor de Internet Information Services (IIS)](iis-server-certificate-installation-instructions.md)
#### [Instrucciones de configuración del directorio virtual](virtual-directory-setup-instructions.md)
#### [Instalación de Message Queuing (MSMQ)](installing-message-queuing-msmq.md)
### [Compilación de los ejemplos de Windows Communication Foundation](building-the-samples.md)
### [Ejecución de los ejemplos de Windows Communication Foundation](running-the-samples.md)
## [Básico](basic.md)
### [Introducción](getting-started-sample.md)
### [AJAX](ajax.md)
#### [JSONP](jsonp.md)
#### [Serialización de JSON](json-serialization.md)
#### [Servicio AJAX básico](basic-ajax-service.md)
#### [Servicio AJAX mediante HTTP POST](ajax-service-using-http-post.md)
#### [Servicio AJAX sin configuración](ajax-service-without-configuration.md)
#### [Servicio AJAX mediante el uso de tipos complejos](ajax-service-using-complex-types-sample.md)
#### [Servicio AJAX con JSON y XML](ajax-service-with-json-and-xml-sample.md)
### [Enlaces](binding.md)
#### [Codificador de ByteStream](bytestream-encoder.md)
#### [Enlace básico](basic-binding.md)
##### [Ejemplo de seguridad de mensaje](message-security-sample.md)
##### [BasicBinding con seguridad de transporte](basicbinding-with-transport-security.md)
##### [BasicBinding](basicbinding.md)
#### [Enlace personalizado](custom-binding.md)
##### [Imperativo en enlace personalizado](custom-binding-imperative.md)
##### [Transporte y codificación de enlace personalizado](custom-binding-transport-and-encoding.md)
##### [Sesión confiable de enlace personalizado](custom-binding-reliable-session.md)
##### [Sesión confiable de enlace personalizado mediante HTTPS](custom-binding-reliable-session-over-https.md)
##### [Seguridad de enlace personalizado](custom-binding-security.md)
#### [Enlace de red](net-binding.md)
##### [Enlace de red MSMQ](net-msmq-binding.md)
###### [Enlace MSMQ por transacciones](transacted-msmq-binding.md)
###### [Comunicación en cola volátil](volatile-queued-communication.md)
###### [Colas de mensajes fallidos](dead-letter-queues.md)
###### [Control de mensajes dudosos en MSMQ 4.0](poison-message-handling-in-msmq-4-0.md)
###### [Sesiones y colas](sessions-and-queues.md)
###### [Comunicación bidireccional](two-way-communication.md)
###### [Procesamiento por lotes con transacciones](transacted-batching.md)
###### [SRMP](srmp.md)
###### [Seguridad de mensajes mediante Message Queuing](message-security-over-message-queuing.md)
###### [Generador de producto de ReceiveContext](receivecontext-enabled-wcf-channels.md)
##### [Integración de Message Queueing](message-queueing-integration.md)
###### [Message Queuing a Windows Communication Foundation](message-queuing-to-wcf.md)
###### [Demux personalizado](custom-demux.md)
###### [Windows Communication Foundation a Message Queuing](wcf-to-message-queuing.md)
###### [Correlación del mensaje](message-correlation.md)
##### [NetTCPBinding](nettcpbinding.md)
###### [NetTcpBinding predeterminado](default-nettcpbinding.md)
###### [Ejemplo de uso compartido de puertos Net.TCP](net-tcp-port-sharing-sample.md)
##### [NetNamedPipeBinding](netnamedpipebinding.md)
#### [Enlace de WS](ws-binding.md)
##### [Enlace HTTP de federación de WS 2007](ws-2007-federation-http-binding.md)
##### [WS Http dual](ws-dual-http.md)
##### [Codificación MTOM](mtom-encoding.md)
##### [WSHttpBinding](wshttpbinding.md)
##### [Sesión de confianza de WS](ws-reliable-session.md)
##### [Seguridad de transporte WS](ws-transport-security.md)
##### [Enlace de seguridad de mensaje](message-security-binding.md)
###### [Seguridad de mensaje anónima](message-security-anonymous.md)
###### [Certificado de seguridad de mensaje](message-security-certificate.md)
###### [Nombre de usuario de seguridad de mensaje](message-security-user-name.md)
###### [Seguridad de mensaje de Windows](message-security-windows.md)
##### [Transporte WS con credencial de mensaje](ws-transport-with-message-credential.md)
##### [Flujo de la transacción WS](ws-transaction-flow.md)
### [Cliente](client.md)
#### [Interoperabilidad de cliente](client-interoperability.md)
##### [Interoperabilidad con servicios web ASMX](interoperating-with-asmx-web-services.md)
##### [Ejemplo de XMLSerializer](xmlserializer-sample.md)
#### [Encabezados de dirección](address-headers.md)
#### [Generador de canales](channel-factory.md)
#### [Excepciones esperadas](expected-exceptions.md)
#### [Recuperación de metadatos](retrieve-metadata.md)
#### [Evitar problemas mediante una declaración de instrucción](avoiding-problems-with-the-using-statement.md)
#### [Cliente con tipo](typed-client.md)
### [Contrato](contract.md)
#### [Contratos de datos](data-contracts.md)
##### [Contrato de datos básico](basic-data-contract.md)
##### [Ejemplo de DataContractSerializer](datacontractserializer-sample.md)
##### [Tipos conocidos](known-types.md)
##### [Referencias a objetos](object-references.md)
##### [Compatibilidad con POCO](poco-support.md)
##### [Uso del enlazador de serialización](usage-of-serialization-binder.md)
#### [Contratos de mensajes](message-contracts.md)
##### [Contrato de mensaje predeterminado](default-message-contract.md)
##### [Solicitud/respuesta sin tipo](untyped-request-reply.md)
##### [Mensajes desajustados](unwrapped-messages.md)
##### [Establecimiento del uso y estilo de las propiedades](setting-the-use-and-style-properties.md)
##### [Ejemplo de XmlReader](xmlreader-sample.md)
#### [Contratos de servicio](service-contracts.md)
##### [Dúplex](duplex.md)
##### [Contrato de error](fault-contract.md)
##### [Unidireccional](one-way.md)
##### [Sesión](session.md)
##### [Secuencia](stream.md)
##### [Errores de XmlSerializer](xmlserializer-faults.md)
#### [DataContractResolver](datacontractresolver.md)
#### [KnownAssemblyAttribute](knownassemblyattribute.md)
#### [Uso de DataContractSerializer y DataContractResolver para proporcionar la funcionalidad de NetDataContractSerializer](datacontractserializer-datacontractresolver-netdatacontractserializer.md)
### [Detección](discovery-samples.md)
#### [Anuncios](announcements-sample.md)
#### [Búsqueda asincrónica](asynchronous-find-sample.md)
#### [Básico](basic-sample.md)
#### [Configuración](configuration-sample.md)
#### [Ejemplo de elemento de enlace de detección](discovery-binding-element-sample.md)
#### [Ejemplo de proxy de detección](discovery-proxy-sample.md)
#### [Ejemplo de detección de un servicio con un modo de URI de escucha único](discover-a-service-with-unique-listen-uri-mode-sample.md)
#### [Detección con ámbitos](discovery-with-scopes-sample.md)
#### [Criterios de búsqueda personalizados](custom-find-criteria.md)
#### [Ejemplo de detección de flujo de trabajo](workflow-discovery-sample.md)
#### [Servicio de enrutador de detección](discovery-router-service.md)
### [Administración](management.md)
#### [Servicios WCF y Seguimiento de eventos para Windows](wcf-services-and-event-tracing-for-windows.md)
#### [Traza analítica de WCF](wcf-analytic-tracing.md)
#### [Seguimiento circular](circular-tracing.md)
#### [Seguimiento ETW](etw-tracing.md)
#### [Extensión del seguimiento](extending-tracing.md)
#### [Bloqueo de seguridad PII](pii-security-lockdown.md)
#### [Uso de contadores de rendimiento](using-performance-counters.md)
#### [Seguimiento y registro de mensajes](tracing-and-message-logging.md)
#### [Validación de seguridad](security-validation.md)
#### [Proveedor WMI](wmi-provider.md)
### [Servicios de enrutamiento](routing-services.md)
#### ["Hola mundo" con el Servicio de enrutamiento](hello-world-with-the-routing-service.md)
#### [Control de errores y puentes](bridging-and-error-handling.md)
#### [Filtros avanzados](advanced-filters.md)
#### [Reconfiguración dinámica](dynamic-reconfiguration.md)
#### [Control de errores avanzado](advanced-error-handling.md)
### [Seguridad](security-in-wcf.md)
#### [Agilidad criptográfica en la seguridad de WCF](cryptographic-agility-in-wcf-security.md)
### [Servicios](services.md)
#### [Hospedar aplicaciones de WPF](hosting.md)
##### [Activación de procesos de Windows](windows-process-activation.md)
###### [Activación NamedPipe](namedpipe-activation.md)
###### [Activación TCP](tcp-activation.md)
###### [Activación MSMQ](msmq-activation.md)
##### [Activación basada en la configuración](configuration-based-activation.md)
##### [Ejemplo de integración de SystemWebRouting](systemwebrouting-integration-sample.md)
##### [Compatibilidad de ASP.NET](aspnet-compatibility.md)
##### [Hospedaje de IIS mediante código en línea](iis-hosting-using-inline-code.md)
##### [Host de servicio de Windows](windows-service-host.md)
##### [Probar internamente](self-host.md)
#### [Interoperabilidad del servicio](service-interoperability.md)
##### [Uso del moniker de WCF con clientes COM](using-the-wcf-moniker-with-com-clients.md)
##### [Cliente ASMX con un servicio WCF](asmx-client-with-a-wcf-service.md)
#### [Comportamientos](behaviors.md)
##### [Simultaneidad](concurrency.md)
##### [Comportamiento de servicio predeterminado](default-service-behavior.md)
##### [Creación de instancias](instancing.md)
##### [Comportamiento de publicación de metadatos](metadata-publishing-behavior.md)
##### [Comportamiento de transacción de servicio](service-transaction-behavior.md)
##### [Comportamiento de depuración de servicio](service-debug-behavior.md)
##### [Limitación de peticiones](throttling.md)
##### [Seguridad de comportamiento](behavior-security.md)
###### [Comportamiento de auditoría de servicio](service-auditing-behavior.md)
###### [Proveedor de pertenencia y roles](membership-and-role-provider.md)
###### [Autorización de acceso a operaciones de servicio](authorizing-access-to-service-operations.md)
###### [Suplantación del cliente](impersonating-the-client.md)
#### [Configuración simplificada de los servicios WCF](simplified-configuration-for-wcf-services.md)
#### [Uso de puntos de conexión estándar](usage-of-standard-endpoints.md)
#### [Modelo de configuración jerárquica](hierarchical-configuration-model.md)
#### [Directiva de protección extendida](extended-protection-policy.md)
#### [Generador de canales de configuración](configuration-channel-factory.md)
#### [Direccionamiento](addressing.md)
#### [Imperativo](imperative.md)
#### [Contratos múltiples](multiple-contracts.md)
#### [Varios puntos de conexión](multiple-endpoints.md)
#### [Varios puntos de conexión en un ListenUri único](multiple-endpoints-at-a-single-listenuri.md)
#### [OperationContextScope](operationcontextscope.md)
#### [Descripción del servicio](service-description.md)
#### [ConcurrencyMode.Reentrant](concurrencymode-reentrant.md)
#### [Seguridad del servicio](service-security.md)
##### [Ejemplo de identidad de servicio](service-identity-sample.md)
### [Redifusión](syndication.md)
#### [Fuente de diagnósticos independientes](stand-alone-diagnostics-feed-sample.md)
#### [Extensiones débilmente tipadas](loosely-typed-extensions-sample.md)
### [Web](web.md)
#### [Selección avanzada de formato](advanced-format-selection.md)
#### [Selección de formato automática](automatic-format-selection.md)
#### [Servicio HTTP básico](basic-http-service.md)
#### [Servicio de recurso básico](basic-resource-service.md)
#### [AspNetRouteIntegration](aspnetrouteintegration.md)
#### [Get y Put condicionales](conditional-get-and-put.md)
#### [Puntos de conexión SOAP y HTTP](soap-and-http-endpoints.md)
#### [Integración de almacenamiento en caché de ASP.NET](aspnet-caching-integration.md)
#### [UriTemplate](uritemplate-sample.md)
#### [Tabla UriTemplate](uritemplate-table-sample.md)
#### [Distribuidor de tabla UriTemplate](uritemplate-table-dispatcher-sample.md)
## [Extensibilidad](extensibility.md)
### [Extensibilidad de enlaces](binding-extensibility.md)
#### [WSStreamedHttpBinding](wsstreamedhttpbinding.md)
### [Extensibilidad de los canales](channels-extensibility.md)
#### [Canal local](local-channel.md)
#### [Perfil seguro confiable](reliable-secure-profile.md)
#### [Distribuidor de canal personalizado](custom-channel-dispatcher.md)
#### [Canal de fragmentación](chunking-channel.md)
#### [Canal de confirmación de HTTP](http-acknowledgement-channel.md)
#### [HttpCookieSession](httpcookiesession.md)
#### [Interceptador de mensajes personalizados](custom-message-interceptor.md)
### [Extensibilidad de la detección](discovery-extensibility.md)
#### [CustomDiscoveryMetadata](customdiscoverymetadata.md)
### [Extensibilidad de creación de instancias](instancing-extensibility.md)
#### [Contexto de instancia duradera](durable-instance-context.md)
#### [Vigencia personalizada](custom-lifetime.md)
#### [Creación de instancias de inicialización](instancing-initialization.md)
#### [Agrupación](pooling.md)
### [Extensibilidad de la interoperabilidad](interop-extensibility.md)
#### [Distribución mediante el elemento del cuerpo](dispatch-by-body-element.md)
#### [Enrutamiento por cuerpo](route-by-body.md)
### [Extensibilidad del codificador de mensajes](message-encoder-extensibility.md)
#### [Codificador de mensaje personalizado: codificador de texto personalizado](custom-message-encoder-custom-text-encoder.md)
#### [Codificador de mensaje personalizado: codificador de compresión](custom-message-encoder-compression-encoder.md)
### [Extensibilidad de metadatos](metadata-extensibility.md)
#### [Punto de conexión personalizado de metadatos seguros](custom-secure-metadata-endpoint.md)
#### [Publicación de WSDL personalizada](custom-wsdl-publication.md)
### [Extensibilidad de la seguridad](security-extensibility.md)
#### [Proveedor de token emitido duradero](durable-issued-token-provider.md)
#### [Proveedor de tokens SAML](saml-token-provider.md)
#### [Tokens auxiliares](supporting-tokens.md)
#### [Autenticador de tokens](token-authenticator.md)
#### [Proveedor de tokens](token-provider.md)
#### [Validador de contraseña de nombre de usuario](user-name-password-validator.md)
#### [Validador de certificado X.509](x-509-certificate-validator.md)
#### [Directiva de autorización](authorization-policy.md)
#### [Token personalizado](custom-token.md)
#### [Validación de cliente](client-validation.md)
### [Ejemplos de extensibilidad de redifusión](syndication-extensibility-samples.md)
#### [Extensiones fuertemente tipadas](strongly-typed-extensions-sample.md)
#### [Formateador de fuentes (JSON)](feed-formatter-json.md)
#### [Fuentes de streaming](streaming-feeds-sample.md)
### [Extensibilidad de transporte](transport-extensibility.md)
#### [Activación UDP](udp-activation.md)
#### [Transporte: transacciones personalizadas sobre UDP](transport-custom-transactions-over-udp-sample.md)
#### [Transporte: UDP](transport-udp.md)
#### [Transporte: interoperabilidad de WSE 3.0 TCP](transport-wse-3-0-tcp-interoperability.md)
### [Extensibilidad web](web-extensibility.md)
#### [Envío de formulario](form-post.md)
### [Formateador de operación y selector de operación](operation-formatter-and-operation-selector.md)
### [Filtro de mensaje personalizado](custom-message-filter.md)
### [Host de servicio personalizado](custom-service-host.md)
### [Suplente de DataContract](datacontract-surrogate.md)
### [Extensión del control sobre el control y los informes de errores](extending-control-over-error-handling-and-reporting.md)
### [Inspectores de mensaje](message-inspectors.md)
### [WebContentTypeMapper](webcontenttypemapper-sample.md)
## [Escenario](scenario.md)
### [Escenarios de enlace de datos](data-binding-scenarios.md)
#### [Enlace de datos en un cliente de Windows Forms](data-binding-in-a-windows-forms-client.md)
#### [Enlace de datos en un cliente ASP.NET](data-binding-in-an-aspnet-client.md)
#### [Enlace de datos en un cliente de Windows Presentation Foundation](data-binding-in-a-wpf-client.md)
### [Ejemplo de seguridad de la detección](discovery-security-sample.md)
### [Ejemplo de federación](federation-sample.md)
### [Ejemplo de serialización JSON débilmente tipada (AJAX)](weakly-typed-json-serialization-sample.md)
### [Servicio de fachada confiable](trusted-facade-service.md)
### [Patrones de diseño: suscripción-publicación basada en la lista](design-patterns-list-based-publish-subscribe.md)
## [Ejemplos de herramientas](tool-samples.md)
### [ConfigurationCodeGenerator](configurationcodegenerator.md)
### [CustomChannelsTester](customchannelstester.md)
### [FindPrivateKey](findprivatekey.md)
