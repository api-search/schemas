---
description: A storage location.
layout: schema
name: StorageLocation
properties_list:
- description: ''
  name: BinaryPrefixLocation
  type: object
- description: ''
  name: Bucket
  type: object
- description: ''
  name: GeneratedPrefixLocation
  type: object
- description: ''
  name: ManifestPrefixLocation
  type: object
- description: ''
  name: RepoPrefixLocation
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-storage-location-schema.json
slug: openapi-storage-location
source_filename: openapi-storage-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-storage-location-schema.json\",\n  \"title\": \"StorageLocation\",\n  \"description\": \"A storage location.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BinaryPrefixLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Object\"\n        },\n        {\n          \"description\": \"The location's binary prefix.\"\n        }\n      ]\n    },\n    \"Bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Bucket\"\n        },\n        {\n          \"description\": \"The location's bucket.\"\n        }\n      ]\n    },\n    \"GeneratedPrefixLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Object\"\n        },\n        {\n          \"description\": \"The location's generated prefix.\"\n\
  \        }\n      ]\n    },\n    \"ManifestPrefixLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Object\"\n        },\n        {\n          \"description\": \"The location's manifest prefix.\"\n        }\n      ]\n    },\n    \"RepoPrefixLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Object\"\n        },\n        {\n          \"description\": \"The location's repo prefix.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"BinaryPrefixLocation\",\n    \"Bucket\",\n    \"GeneratedPrefixLocation\",\n    \"ManifestPrefixLocation\",\n    \"RepoPrefixLocation\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-storage-location-schema.json
tags:
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: StorageLocation
---
