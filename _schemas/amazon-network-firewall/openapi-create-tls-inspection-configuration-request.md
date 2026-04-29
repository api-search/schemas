---
description: CreateTLSInspectionConfigurationRequest schema from Amazon Network Firewall
layout: schema
name: CreateTLSInspectionConfigurationRequest
properties_list:
- description: ''
  name: TLSInspectionConfigurationName
  type: object
- description: ''
  name: TLSInspectionConfiguration
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: EncryptionConfiguration
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-create-tls-inspection-configuration-request-schema.json
slug: openapi-create-tls-inspection-configuration-request
source_filename: openapi-create-tls-inspection-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-create-tls-inspection-configuration-request-schema.json\",\n  \"title\": \"CreateTLSInspectionConfigurationRequest\",\n  \"description\": \"CreateTLSInspectionConfigurationRequest schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TLSInspectionConfigurationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The descriptive name of the TLS inspection configuration. You can't change the name of a TLS inspection configuration after you create it.\"\n        }\n      ]\n    },\n    \"TLSInspectionConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TLSInspectionConfiguration\"\n        },\n        {\n         \
  \ \"description\": \"<p>The object that defines a TLS inspection configuration. This, along with <a>TLSInspectionConfigurationResponse</a>, define the TLS inspection configuration. You can retrieve all objects for a TLS inspection configuration by calling <a>DescribeTLSInspectionConfiguration</a>. </p> <p>Network Firewall uses a TLS inspection configuration to decrypt traffic. Network Firewall re-encrypts the traffic before sending it to its destination.</p> <p>To use a TLS inspection configuration, you add it to a Network Firewall firewall policy, then you apply the firewall policy to a firewall. Network Firewall acts as a proxy service to decrypt and inspect inbound traffic. You can reference a TLS inspection configuration from more than one firewall policy, and you can use a firewall policy in more than one firewall. For more information about using TLS inspection configurations, see <a href=\\\"https://docs.aws.amazon.com/network-firewall/latest/developerguide/tls-inspection.html\\\
  \">Decrypting SSL/TLS traffic with TLS inspection configurations</a> in the <i>Network Firewall Developer Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description of the TLS inspection configuration. \"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The key:value pairs to associate with the resource.\"\n        }\n      ]\n    },\n    \"EncryptionConfiguration\": {\n      \"$ref\": \"#/components/schemas/EncryptionConfiguration\"\n    }\n  },\n  \"required\": [\n    \"TLSInspectionConfigurationName\",\n    \"TLSInspectionConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-create-tls-inspection-configuration-request-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: CreateTLSInspectionConfigurationRequest
---
