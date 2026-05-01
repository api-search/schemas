---
description: Details about the query.
layout: schema
name: QueryInfo
properties_list:
- description: ''
  name: SelectFields
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-query-info-schema.json
slug: config-query-info
source_filename: config-query-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-query-info-schema.json\",\n  \"title\": \"QueryInfo\",\n  \"description\": \"Details about the query.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SelectFields\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FieldInfoList\"\n        },\n        {\n          \"description\": \"Returns a <code>FieldInfo</code> object.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-query-info-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: QueryInfo
---
