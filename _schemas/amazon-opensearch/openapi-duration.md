---
description: 'Specifies maintenance schedule duration: duration value and duration unit. See the <a href="https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/auto-tune.html" target="_blank">Developer Guide</a> for more information.'
layout: schema
name: Duration
properties_list:
- description: ''
  name: Value
  type: object
- description: ''
  name: Unit
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-duration-schema.json
slug: openapi-duration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-duration-schema.json\",\n  \"title\": \"Duration\",\n  \"description\": \"Specifies maintenance schedule duration: duration value and duration unit. See the <a href=\\\"https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/auto-tune.html\\\" target=\\\"_blank\\\">Developer Guide</a> for more information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationValue\"\n        },\n        {\n          \"description\": \" Integer to specify the value of a maintenance schedule duration. See the <a href=\\\"https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/auto-tune.html\\\" target=\\\"_blank\\\">Developer Guide</a> for more information.\"\n        }\n      ]\n   \
  \ },\n    \"Unit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeUnit\"\n        },\n        {\n          \"description\": \"Specifies the unit of a maintenance schedule duration. Valid value is HOURS. See the <a href=\\\"https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/auto-tune.html\\\" target=\\\"_blank\\\">Developer Guide</a> for more information.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-duration-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: Duration
---
