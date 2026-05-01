---
description: Specifies Auto-Tune type and Auto-Tune action details.
layout: schema
name: AutoTune
properties_list:
- description: ''
  name: AutoTuneType
  type: object
- description: ''
  name: AutoTuneDetails
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-auto-tune-schema.json
slug: openapi-auto-tune
source_filename: openapi-auto-tune-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-auto-tune-schema.json\",\n  \"title\": \"AutoTune\",\n  \"description\": \"Specifies Auto-Tune type and Auto-Tune action details. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoTuneType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoTuneType\"\n        },\n        {\n          \"description\": \"Specifies Auto-Tune type. Valid value is SCHEDULED_ACTION. \"\n        }\n      ]\n    },\n    \"AutoTuneDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoTuneDetails\"\n        },\n        {\n          \"description\": \"Specifies details of the Auto-Tune action. See the <a href=\\\"https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/auto-tune.html\\\" target=\\\"_blank\\\">Developer Guide</a>\
  \ for more information. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-auto-tune-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: AutoTune
---
