---
description: UpdateLoggingConfigurationResponse schema from Amazon Network Firewall
layout: schema
name: UpdateLoggingConfigurationResponse
properties_list:
- description: ''
  name: FirewallArn
  type: object
- description: ''
  name: FirewallName
  type: object
- description: ''
  name: LoggingConfiguration
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-update-logging-configuration-response-schema.json
slug: openapi-update-logging-configuration-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-update-logging-configuration-response-schema.json\",\n  \"title\": \"UpdateLoggingConfigurationResponse\",\n  \"description\": \"UpdateLoggingConfigurationResponse schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FirewallArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the firewall.\"\n        }\n      ]\n    },\n    \"FirewallName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The descriptive name of the firewall. You can't change the name of a firewall after you create it.\"\n        }\n      ]\n    },\n    \"\
  LoggingConfiguration\": {\n      \"$ref\": \"#/components/schemas/LoggingConfiguration\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-update-logging-configuration-response-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: UpdateLoggingConfigurationResponse
---
