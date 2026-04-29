---
description: 'Specifies the Auto-Tune options: the Auto-Tune desired state for the domain and list of maintenance schedules.'
layout: schema
name: AutoTuneOptionsOutput
properties_list:
- description: ''
  name: State
  type: object
- description: ''
  name: ErrorMessage
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-auto-tune-options-output-schema.json
slug: openapi-auto-tune-options-output
source_filename: openapi-auto-tune-options-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-auto-tune-options-output-schema.json\",\n  \"title\": \"AutoTuneOptionsOutput\",\n  \"description\": \"Specifies the Auto-Tune options: the Auto-Tune desired state for the domain and list of maintenance schedules.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoTuneState\"\n        },\n        {\n          \"description\": \"Specifies the <code>AutoTuneState</code> for the Elasticsearch domain.\"\n        }\n      ]\n    },\n    \"ErrorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Specifies the error message while enabling or disabling the Auto-Tune.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-auto-tune-options-output-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: AutoTuneOptionsOutput
---
