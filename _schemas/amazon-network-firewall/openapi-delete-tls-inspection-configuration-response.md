---
description: DeleteTLSInspectionConfigurationResponse schema from Amazon Network Firewall
layout: schema
name: DeleteTLSInspectionConfigurationResponse
properties_list:
- description: ''
  name: TLSInspectionConfigurationResponse
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-delete-tls-inspection-configuration-response-schema.json
slug: openapi-delete-tls-inspection-configuration-response
source_filename: openapi-delete-tls-inspection-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-delete-tls-inspection-configuration-response-schema.json\",\n  \"title\": \"DeleteTLSInspectionConfigurationResponse\",\n  \"description\": \"DeleteTLSInspectionConfigurationResponse schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TLSInspectionConfigurationResponse\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TLSInspectionConfigurationResponse\"\n        },\n        {\n          \"description\": \"The high-level properties of a TLS inspection configuration. This, along with the <a>TLSInspectionConfiguration</a>, define the TLS inspection configuration. You can retrieve all objects for a TLS inspection configuration by calling <a>DescribeTLSInspectionConfiguration</a>. \"\n        }\n      ]\n    }\n  },\n  \"\
  required\": [\n    \"TLSInspectionConfigurationResponse\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-delete-tls-inspection-configuration-response-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: DeleteTLSInspectionConfigurationResponse
---
