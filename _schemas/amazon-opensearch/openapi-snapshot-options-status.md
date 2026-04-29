---
description: Status of a daily automated snapshot.
layout: schema
name: SnapshotOptionsStatus
properties_list:
- description: ''
  name: Options
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-snapshot-options-status-schema.json
slug: openapi-snapshot-options-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-snapshot-options-status-schema.json\",\n  \"title\": \"SnapshotOptionsStatus\",\n  \"description\": \"Status of a daily automated snapshot.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Options\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnapshotOptions\"\n        },\n        {\n          \"description\": \"Specifies the daily snapshot options specified for the Elasticsearch domain.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OptionStatus\"\n        },\n        {\n          \"description\": \"Specifies the status of a daily automated snapshot.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Options\",\n    \"Status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-snapshot-options-status-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: SnapshotOptionsStatus
---
