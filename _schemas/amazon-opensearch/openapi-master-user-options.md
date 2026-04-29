---
description: 'Credentials for the master user: username and password, ARN, or both.'
layout: schema
name: MasterUserOptions
properties_list:
- description: ''
  name: MasterUserARN
  type: object
- description: ''
  name: MasterUserName
  type: object
- description: ''
  name: MasterUserPassword
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-master-user-options-schema.json
slug: openapi-master-user-options
source_filename: openapi-master-user-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-master-user-options-schema.json\",\n  \"title\": \"MasterUserOptions\",\n  \"description\": \"Credentials for the master user: username and password, ARN, or both.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MasterUserARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"ARN for the master user (if IAM is enabled).\"\n        }\n      ]\n    },\n    \"MasterUserName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Username\"\n        },\n        {\n          \"description\": \"The master user's username, which is stored in the Amazon Elasticsearch Service domain's internal database.\"\n        }\n      ]\n    },\n    \"MasterUserPassword\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/Password\"\n        },\n        {\n          \"description\": \"The master user's password, which is stored in the Amazon Elasticsearch Service domain's internal database.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-master-user-options-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: MasterUserOptions
---
