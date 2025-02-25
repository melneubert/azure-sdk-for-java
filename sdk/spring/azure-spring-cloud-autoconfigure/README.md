# Spring Cloud for Azure AutoConfigure client library for Java
This package is for Spring Cloud Starters of Azure services. It helps Spring Cloud developers to adopt Azure services.

[Source code][src] | [Package (Maven)][package] | [API reference documentation][refdocs]

## Getting started

### Prerequisites
- [Environment checklist][environment_checklist]

### Include the Package
1. [Add azure-spring-cloud-dependencies].
1. Add dependency. `<version>` can be skipped because we already add `azure-spring-cloud-dependencies`.
```xml
<dependency>
  <groupId>com.azure.spring</groupId>
  <artifactId>azure-spring-cloud-autoconfigure</artifactId>
</dependency>
```

## Key concepts
This project provides auto-configuration for the following Azure services:

- [Azure App Configuration][app_configuration]
- [Azure Cache][cache]
- [Event Hubs][event_hubs]
- [Event Hubs Kafka][event_hubs_kafka]
- [Service Bus][service_bus]
- [Storage Queue][storage_queue]

## Examples

The following section provides sample projects illustrating how to use the Spring Cloud for Azure starters.
### More sample code
- [Azure App Configuration][app_configuration_sample]
- [Azure App Configuration Conversation][app_configuration_conversation_sample]
- [Azure Cache][cache_sample]
- [Event Hubs][event_hubs_sample]
- [Event Hubs Kafka][event_hubs_kafka_sample]
- [Service Bus][service_bus_sample]
- [Storage Queue][storage_queue_sample]

## Troubleshooting
### Enable client logging
Azure SDKs for Java offers a consistent logging story to help aid in troubleshooting application errors and expedite their resolution. The logs produced will capture the flow of an application before reaching the terminal state to help locate the root issue. View the [logging][logging] wiki for guidance about enabling logging.

### Enable Spring logging
Spring allow all the supported logging systems to set logger levels set in the Spring Environment (for example, in application.properties) by using `logging.level.<logger-name>=<level>` where level is one of TRACE, DEBUG, INFO, WARN, ERROR, FATAL, or OFF. The root logger can be configured by using logging.level.root.

The following example shows potential logging settings in `application.properties`:

```properties
logging.level.root=WARN
logging.level.org.springframework.web=DEBUG
logging.level.org.hibernate=ERROR
```

For more information about setting logging in spring, please refer to the [official doc][logging_doc].
 

## Next steps

The following section provides sample projects illustrating how to use the Spring Cloud for Azure starters.
### More sample code
- [Azure App Configuration][app_configuration_sample]
- [Azure App Configuration Conversation][app_configuration_conversation_sample]
- [Azure Cache][cache_sample]
- [Event Hubs][event_hubs_sample]
- [Event Hubs Kafka][event_hubs_kafka_sample]
- [Service Bus][service_bus_sample]
- [Storage Queue][storage_queue_sample]

## Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us the rights to use your contribution. For details, visit https://cla.microsoft.com.

Please follow [instructions here][contributing_md] to build from source or contribute.

<!-- Link -->
[src]: https://github.com/Azure/azure-sdk-for-java/tree/main/sdk/spring/azure-spring-cloud-autoconfigure/src/
[package]: https://mvnrepository.com/artifact/com.azure.spring/azure-spring-cloud-autoconfigure
[refdocs]: https://azure.github.io/azure-sdk-for-java/springcloud.html#azure-spring-cloud-autoconfigure
[logging]: https://github.com/Azure/azure-sdk-for-java/wiki/Logging-with-Azure-SDK#use-logback-logging-framework-in-a-spring-boot-application
[spring_io]: https://start.spring.io
[logging_doc]: https://docs.spring.io/spring-boot/docs/current/reference/html/features.html#boot-features-logging
[contributing_md]: https://github.com/Azure/azure-sdk-for-java/tree/main/sdk/spring/CONTRIBUTING.md
[maven]: https://maven.apache.org/
[app_configuration]: https://github.com/Azure/azure-sdk-for-java/tree/main/sdk/appconfiguration/spring-cloud-starter-azure-appconfiguration-config
[cache]: https://github.com/Azure/azure-sdk-for-java/tree/main/sdk/spring/azure-spring-cloud-starter-cache
[event_hubs]: https://github.com/Azure/azure-sdk-for-java/tree/main/sdk/spring/azure-spring-cloud-starter-eventhubs
[event_hubs_kafka]: https://github.com/Azure/azure-sdk-for-java/tree/main/sdk/spring/azure-spring-cloud-starter-eventhubs-kafka
[service_bus]: https://github.com/Azure/azure-sdk-for-java/tree/main/sdk/spring/azure-spring-cloud-starter-servicebus
[storage_queue]: https://github.com/Azure/azure-sdk-for-java/tree/main/sdk/spring/azure-spring-cloud-starter-storage-queue
[app_configuration_sample]: https://github.com/Azure-Samples/azure-spring-boot-samples/tree/tag_azure-spring-boot_3.6.0/appconfiguration/azure-appconfiguration-sample
[app_configuration_conversation_sample]: https://github.com/Azure-Samples/azure-spring-boot-samples/tree/tag_azure-spring-boot_3.6.0/appconfiguration/azure-appconfiguration-conversion-sample-complete
[cache_sample]: https://github.com/Azure-Samples/azure-spring-boot-samples/tree/tag_azure-spring-boot_3.6.0/cache/azure-spring-cloud-sample-cache
[event_hubs_sample]: https://github.com/Azure-Samples/azure-spring-boot-samples/tree/tag_azure-spring-boot_3.6.0/eventhubs/azure-spring-integration-sample-eventhubs
[event_hubs_kafka_sample]: https://github.com/Azure-Samples/azure-spring-boot-samples/tree/tag_azure-spring-boot_3.6.0/eventhubs/azure-spring-cloud-sample-eventhubs-kafka
[service_bus_sample]: https://github.com/Azure-Samples/azure-spring-boot-samples/tree/tag_azure-spring-boot_3.6.0/servicebus/azure-spring-integration-sample-servicebus
[storage_queue_sample]: https://github.com/Azure-Samples/azure-spring-boot-samples/tree/tag_azure-spring-boot_3.6.0/storage/azure-spring-integration-sample-storage-queue
[environment_checklist]: https://github.com/Azure/azure-sdk-for-java/blob/main/sdk/spring/ENVIRONMENT_CHECKLIST.md#ready-to-run-checklist
[Add azure-spring-cloud-dependencies]: https://github.com/Azure/azure-sdk-for-java/blob/main/sdk/spring/AZURE_SPRING_BOMS_USAGE.md#add-azure-spring-cloud-dependencies
