---
description: Provides the current status of the entity.
layout: schema
name: OptionStatus
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
  name: PendingDeletion
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-option-status-schema.json
slug: openapi-option-status
source_filename: openapi-option-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-option-status-schema.json\",\n  \"title\": \"OptionStatus\",\n  \"description\": \"Provides the current status of the entity.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateTimestamp\"\n        },\n        {\n          \"description\": \"Timestamp which tells the creation date for the entity.\"\n        }\n      ]\n    },\n    \"UpdateDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateTimestamp\"\n        },\n        {\n          \"description\": \"Timestamp which tells the last updated time for the entity.\"\n        }\n      ]\n    },\n    \"UpdateVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UIntValue\"\
  \n        },\n        {\n          \"description\": \"Specifies the latest version for the entity.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OptionState\"\n        },\n        {\n          \"description\": \"Provides the <code>OptionState</code> for the Elasticsearch domain.\"\n        }\n      ]\n    },\n    \"PendingDeletion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Indicates whether the Elasticsearch domain is being deleted.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CreationDate\",\n    \"UpdateDate\",\n    \"State\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-option-status-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: OptionStatus
---
