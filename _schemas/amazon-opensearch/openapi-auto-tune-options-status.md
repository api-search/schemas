---
description: Specifies the status of Auto-Tune options for the specified Elasticsearch domain.
layout: schema
name: AutoTuneOptionsStatus
properties_list:
- description: ''
  name: Options
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-auto-tune-options-status-schema.json
slug: openapi-auto-tune-options-status
source_filename: openapi-auto-tune-options-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-auto-tune-options-status-schema.json\",\n  \"title\": \"AutoTuneOptionsStatus\",\n  \"description\": \" Specifies the status of Auto-Tune options for the specified Elasticsearch domain.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Options\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoTuneOptions\"\n        },\n        {\n          \"description\": \" Specifies Auto-Tune options for the specified Elasticsearch domain.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoTuneStatus\"\n        },\n        {\n          \"description\": \" Specifies Status of the Auto-Tune options for the specified Elasticsearch domain.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-auto-tune-options-status-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: AutoTuneOptionsStatus
---
