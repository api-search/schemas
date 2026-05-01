---
description: A Dynamic Adaptive Streaming over HTTP (DASH) encryption configuration.
layout: schema
name: DashEncryption
properties_list:
- description: ''
  name: KeyRotationIntervalSeconds
  type: object
- description: ''
  name: SpekeKeyProvider
  type: object
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-dash-encryption-schema.json
slug: mediapackage-api-dash-encryption
source_filename: mediapackage-api-dash-encryption-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-dash-encryption-schema.json\",\n  \"title\": \"DashEncryption\",\n  \"description\": \"A Dynamic Adaptive Streaming over HTTP (DASH) encryption configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"KeyRotationIntervalSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"keyRotationIntervalSeconds\"\n          },\n          \"description\": \"Time (in seconds) between each encryption key rotation.\"\n        }\n      ]\n    },\n    \"SpekeKeyProvider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SpekeKeyProvider\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"spekeKeyProvider\"\n          }\n  \
  \      }\n      ]\n    }\n  },\n  \"required\": [\n    \"SpekeKeyProvider\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-dash-encryption-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: DashEncryption
---
