---
description: DescribeDomainConfigurationResponse schema
layout: schema
name: DescribeDomainConfigurationResponse
properties_list:
- description: ''
  name: domainConfigurationName
  type: object
- description: ''
  name: domainConfigurationArn
  type: object
- description: ''
  name: domainName
  type: object
- description: ''
  name: serverCertificates
  type: object
- description: ''
  name: authorizerConfig
  type: object
- description: ''
  name: domainConfigurationStatus
  type: object
- description: ''
  name: serviceType
  type: object
- description: ''
  name: domainType
  type: object
- description: ''
  name: lastStatusChangeDate
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-describe-domain-configuration-response-schema.json
slug: iot-device-management-describe-domain-configuration-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-domain-configuration-response-schema.json\",\n  \"title\": \"DescribeDomainConfigurationResponse\",\n  \"description\": \"DescribeDomainConfigurationResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domainConfigurationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReservedDomainConfigurationName\"\n        },\n        {\n          \"description\": \"The name of the domain configuration.\"\n        }\n      ]\n    },\n    \"domainConfigurationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainConfigurationArn\"\n        },\n        {\n          \"description\": \"The ARN of the domain configuration.\"\n        }\n      ]\n    },\n    \"domainName\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The name of the domain.\"\n        }\n      ]\n    },\n    \"serverCertificates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServerCertificates\"\n        },\n        {\n          \"description\": \"A list containing summary information about the server certificate included in the domain configuration.\"\n        }\n      ]\n    },\n    \"authorizerConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthorizerConfig\"\n        },\n        {\n          \"description\": \"An object that specifies the authorization service for a domain.\"\n        }\n      ]\n    },\n    \"domainConfigurationStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainConfigurationStatus\"\n        },\n        {\n          \"description\": \"A Boolean value that specifies the current\
  \ state of the domain configuration.\"\n        }\n      ]\n    },\n    \"serviceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceType\"\n        },\n        {\n          \"description\": \"The type of service delivered by the endpoint.\"\n        }\n      ]\n    },\n    \"domainType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainType\"\n        },\n        {\n          \"description\": \"The type of the domain.\"\n        }\n      ]\n    },\n    \"lastStatusChangeDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The date and time the domain configuration's status was last changed.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-domain-configuration-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: DescribeDomainConfigurationResponse
---
