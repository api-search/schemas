---
description: Provides the current status of the Auto-Tune options.
layout: schema
name: AutoTuneStatus
properties_list:
- description: ''
  name: CreationDate
  type: object
- description: ''
  name: UpdateDate
  type: object
- description: ''
  name: UpdateVersion
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: ErrorMessage
  type: object
- description: ''
  name: PendingDeletion
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-auto-tune-status-schema.json
slug: openapi-auto-tune-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-auto-tune-status-schema.json\",\n  \"title\": \"AutoTuneStatus\",\n  \"description\": \"Provides the current status of the Auto-Tune options. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateTimestamp\"\n        },\n        {\n          \"description\": \"Timestamp which tells Auto-Tune options creation date .\"\n        }\n      ]\n    },\n    \"UpdateDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateTimestamp\"\n        },\n        {\n          \"description\": \"Timestamp which tells Auto-Tune options last updated time.\"\n        }\n      ]\n    },\n    \"UpdateVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UIntValue\"\
  \n        },\n        {\n          \"description\": \"Specifies the Auto-Tune options latest version.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoTuneState\"\n        },\n        {\n          \"description\": \"Specifies the <code>AutoTuneState</code> for the Elasticsearch domain.\"\n        }\n      ]\n    },\n    \"ErrorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Specifies the error message while enabling or disabling the Auto-Tune options.\"\n        }\n      ]\n    },\n    \"PendingDeletion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Indicates whether the Elasticsearch domain is being deleted.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CreationDate\",\n    \"UpdateDate\",\n    \"State\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-auto-tune-status-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: AutoTuneStatus
---
