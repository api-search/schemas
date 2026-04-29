---
description: CreateDomainConfigurationResponse schema
layout: schema
name: CreateDomainConfigurationResponse
properties_list:
- description: ''
  name: domainConfigurationName
  type: object
- description: ''
  name: domainConfigurationArn
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-create-domain-configuration-response-schema.json
slug: iot-device-defender-create-domain-configuration-response
source_filename: iot-device-defender-create-domain-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-create-domain-configuration-response-schema.json\",\n  \"title\": \"CreateDomainConfigurationResponse\",\n  \"description\": \"CreateDomainConfigurationResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domainConfigurationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainConfigurationName\"\n        },\n        {\n          \"description\": \"The name of the domain configuration.\"\n        }\n      ]\n    },\n    \"domainConfigurationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainConfigurationArn\"\n        },\n        {\n          \"description\": \"The ARN of the domain configuration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-create-domain-configuration-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: CreateDomainConfigurationResponse
---
