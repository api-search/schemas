---
description: DescribeTLSInspectionConfigurationRequest schema from Amazon Network Firewall
layout: schema
name: DescribeTLSInspectionConfigurationRequest
properties_list:
- description: ''
  name: TLSInspectionConfigurationArn
  type: object
- description: ''
  name: TLSInspectionConfigurationName
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-describe-tls-inspection-configuration-request-schema.json
slug: openapi-describe-tls-inspection-configuration-request
source_filename: openapi-describe-tls-inspection-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-describe-tls-inspection-configuration-request-schema.json\",\n  \"title\": \"DescribeTLSInspectionConfigurationRequest\",\n  \"description\": \"DescribeTLSInspectionConfigurationRequest schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TLSInspectionConfigurationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the TLS inspection configuration.</p> <p>You must specify the ARN or the name, and you can specify both. </p>\"\n        }\n      ]\n    },\n    \"TLSInspectionConfigurationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n       \
  \   \"description\": \"<p>The descriptive name of the TLS inspection configuration. You can't change the name of a TLS inspection configuration after you create it.</p> <p>You must specify the ARN or the name, and you can specify both. </p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-describe-tls-inspection-configuration-request-schema.json
tags:
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: DescribeTLSInspectionConfigurationRequest
---
