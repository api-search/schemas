---
description: Contains details about a package version asset.
layout: schema
name: AssetSummary
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: size
  type: object
- description: ''
  name: hashes
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-asset-summary-schema.json
slug: codeartifact-asset-summary
source_filename: codeartifact-asset-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-asset-summary-schema.json\",\n  \"title\": \"AssetSummary\",\n  \"description\": \" Contains details about a package version asset. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetName\"\n        },\n        {\n          \"description\": \" The name of the asset. \"\n        }\n      ]\n    },\n    \"size\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongOptional\"\n        },\n        {\n          \"description\": \" The size of the asset. \"\n        }\n      ]\n    },\n    \"hashes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetHashes\"\n        },\n        {\n          \"description\": \" The hashes of the asset.\
  \ \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-asset-summary-schema.json
tags:
- Amazon
- AWS
- Artifact Repository
- Package Management
- DevOps
- Software Supply Chain
- npm
- Maven
- PyPI
- NuGet
title: AssetSummary
---
