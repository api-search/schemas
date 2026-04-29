---
description: Schema for a container image analyzed by Anchore Enterprise
layout: schema
name: Anchore Image
properties_list:
- description: SHA256 digest of the image
  name: imageDigest
  type: string
- description: ''
  name: analysisStatus
  type: string
- description: ''
  name: imageStatus
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
- description: ''
  name: imageContent
  type: object
provider_name: Anchore
provider_slug: anchore
schema_file: json-schema/anchore-image-schema.json
slug: anchore-image
source_filename: anchore-image-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/anchore/refs/heads/main/json-schema/anchore-image-schema.json\",\n  \"title\": \"Anchore Image\",\n  \"description\": \"Schema for a container image analyzed by Anchore Enterprise\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"imageDigest\": {\n      \"type\": \"string\",\n      \"description\": \"SHA256 digest of the image\"\n    },\n    \"analysisStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"not_analyzed\",\n        \"analyzing\",\n        \"analyzed\",\n        \"analysis_failed\"\n      ]\n    },\n    \"imageStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"active\",\n        \"inactive\",\n        \"deleting\"\n      ]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\":\
  \ \"date-time\"\n    },\n    \"imageContent\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"metadata\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"arch\": {\n              \"type\": \"string\"\n            },\n            \"distro\": {\n              \"type\": \"string\"\n            },\n            \"distroVersion\": {\n              \"type\": \"string\"\n            },\n            \"imageSize\": {\n              \"type\": \"integer\"\n            },\n            \"layerCount\": {\n              \"type\": \"integer\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"imageDigest\",\n    \"analysisStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/anchore/refs/heads/main/json-schema/anchore-image-schema.json
tags:
- Container Security
- Containers
- SBOM
- Software Supply Chain
- Vulnerability Scanning
title: Anchore Image
---
