---
description: A progress stage details of a specific domain configuration change.
layout: schema
name: ChangeProgressStage
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: LastUpdated
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-change-progress-stage-schema.json
slug: openapi-change-progress-stage
source_filename: openapi-change-progress-stage-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-change-progress-stage-schema.json\",\n  \"title\": \"ChangeProgressStage\",\n  \"description\": \"A progress stage details of a specific domain configuration change.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChangeProgressStageName\"\n        },\n        {\n          \"description\": \"The name of the specific progress stage.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChangeProgressStageStatus\"\n        },\n        {\n          \"description\": \"The overall status of a specific progress stage.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\
  \n        },\n        {\n          \"description\": \"The description of the progress stage.\"\n        }\n      ]\n    },\n    \"LastUpdated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastUpdated\"\n        },\n        {\n          \"description\": \"The last updated timestamp of the progress stage.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-change-progress-stage-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: ChangeProgressStage
---
