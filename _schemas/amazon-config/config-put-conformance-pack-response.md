---
description: PutConformancePackResponse schema
layout: schema
name: PutConformancePackResponse
properties_list:
- description: ''
  name: ConformancePackArn
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-put-conformance-pack-response-schema.json
slug: config-put-conformance-pack-response
source_filename: config-put-conformance-pack-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-conformance-pack-response-schema.json\",\n  \"title\": \"PutConformancePackResponse\",\n  \"description\": \"PutConformancePackResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConformancePackArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackArn\"\n        },\n        {\n          \"description\": \"ARN of the conformance pack.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-conformance-pack-response-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: PutConformancePackResponse
---
