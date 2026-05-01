---
description: DeleteConformancePackRequest schema
layout: schema
name: DeleteConformancePackRequest
properties_list:
- description: ''
  name: ConformancePackName
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-delete-conformance-pack-request-schema.json
slug: config-delete-conformance-pack-request
source_filename: config-delete-conformance-pack-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-delete-conformance-pack-request-schema.json\",\n  \"title\": \"DeleteConformancePackRequest\",\n  \"description\": \"DeleteConformancePackRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConformancePackName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackName\"\n        },\n        {\n          \"description\": \"Name of the conformance pack you want to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConformancePackName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-delete-conformance-pack-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: DeleteConformancePackRequest
---
