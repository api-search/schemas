---
description: Specifies change details of the domain configuration change.
layout: schema
name: ChangeProgressDetails
properties_list:
- description: ''
  name: ChangeId
  type: object
- description: ''
  name: Message
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-change-progress-details-schema.json
slug: openapi-change-progress-details
source_filename: openapi-change-progress-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-change-progress-details-schema.json\",\n  \"title\": \"ChangeProgressDetails\",\n  \"description\": \"Specifies change details of the domain configuration change.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChangeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GUID\"\n        },\n        {\n          \"description\": \"The unique change identifier associated with a specific domain configuration change.\"\n        }\n      ]\n    },\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Message\"\n        },\n        {\n          \"description\": \"Contains an optional message associated with the domain configuration change.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-change-progress-details-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: ChangeProgressDetails
---
