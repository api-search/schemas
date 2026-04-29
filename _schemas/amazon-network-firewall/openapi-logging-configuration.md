---
description: Defines how Network Firewall performs logging for a <a>Firewall</a>.
layout: schema
name: LoggingConfiguration
properties_list:
- description: ''
  name: LogDestinationConfigs
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-logging-configuration-schema.json
slug: openapi-logging-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-logging-configuration-schema.json\",\n  \"title\": \"LoggingConfiguration\",\n  \"description\": \"Defines how Network Firewall performs logging for a <a>Firewall</a>. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LogDestinationConfigs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogDestinationConfigs\"\n        },\n        {\n          \"description\": \"Defines the logging destinations for the logs for a firewall. Network Firewall generates logs for stateful rule groups. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LogDestinationConfigs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-logging-configuration-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: LoggingConfiguration
---
