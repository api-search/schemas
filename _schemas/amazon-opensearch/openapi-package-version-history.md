---
description: Details of a package version.
layout: schema
name: PackageVersionHistory
properties_list:
- description: ''
  name: PackageVersion
  type: object
- description: ''
  name: CommitMessage
  type: object
- description: ''
  name: CreatedAt
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-package-version-history-schema.json
slug: openapi-package-version-history
source_filename: openapi-package-version-history-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-package-version-history-schema.json\",\n  \"title\": \"PackageVersionHistory\",\n  \"description\": \"Details of a package version.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PackageVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersion\"\n        },\n        {\n          \"description\": \"Version of the package.\"\n        }\n      ]\n    },\n    \"CommitMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CommitMessage\"\n        },\n        {\n          \"description\": \"A message associated with the version.\"\n        }\n      ]\n    },\n    \"CreatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedAt\"\n        },\n        {\n          \"description\"\
  : \"Timestamp which tells creation time of the package version.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-package-version-history-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: PackageVersionHistory
---
