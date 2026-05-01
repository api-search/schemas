---
description: TagResourceRequest schema
layout: schema
name: TagResourceRequest
properties_list:
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-tag-resource-request-schema.json
slug: config-tag-resource-request
source_filename: config-tag-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-tag-resource-request-schema.json\",\n  \"title\": \"TagResourceRequest\",\n  \"description\": \"TagResourceRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that identifies the resource for which to list the tags. Currently, the supported resources are <code>ConfigRule</code>, <code>ConfigurationAggregator</code> and <code>AggregatorAuthorization</code>.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"An array of tag object.\"\n        }\n      ]\n\
  \    }\n  },\n  \"required\": [\n    \"ResourceArn\",\n    \"Tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-tag-resource-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: TagResourceRequest
---
