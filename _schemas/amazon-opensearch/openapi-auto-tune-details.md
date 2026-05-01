---
description: Specifies details of the Auto-Tune action. See the <a href="https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/auto-tune.html" target="_blank">Developer Guide</a> for more information.
layout: schema
name: AutoTuneDetails
properties_list:
- description: ''
  name: ScheduledAutoTuneDetails
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-auto-tune-details-schema.json
slug: openapi-auto-tune-details
source_filename: openapi-auto-tune-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-auto-tune-details-schema.json\",\n  \"title\": \"AutoTuneDetails\",\n  \"description\": \"Specifies details of the Auto-Tune action. See the <a href=\\\"https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/auto-tune.html\\\" target=\\\"_blank\\\">Developer Guide</a> for more information. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ScheduledAutoTuneDetails\": {\n      \"$ref\": \"#/components/schemas/ScheduledAutoTuneDetails\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-auto-tune-details-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: AutoTuneDetails
---
