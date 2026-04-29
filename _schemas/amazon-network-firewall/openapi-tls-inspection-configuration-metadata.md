---
description: High-level information about a TLS inspection configuration, returned by <code>ListTLSInspectionConfigurations</code>. You can use the information provided in the metadata to retrieve and manage a TLS configuration.
layout: schema
name: TLSInspectionConfigurationMetadata
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Arn
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-tls-inspection-configuration-metadata-schema.json
slug: openapi-tls-inspection-configuration-metadata
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-tls-inspection-configuration-metadata-schema.json\",\n  \"title\": \"TLSInspectionConfigurationMetadata\",\n  \"description\": \"High-level information about a TLS inspection configuration, returned by <code>ListTLSInspectionConfigurations</code>. You can use the information provided in the metadata to retrieve and manage a TLS configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The descriptive name of the TLS inspection configuration. You can't change the name of a TLS inspection configuration after you create it.\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\
  \n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the TLS inspection configuration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-tls-inspection-configuration-metadata-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: TLSInspectionConfigurationMetadata
---
