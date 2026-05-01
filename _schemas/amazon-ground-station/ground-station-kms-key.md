---
description: AWS Key Management Service (KMS) Key.
layout: schema
name: KmsKey
properties_list:
- description: ''
  name: kmsAliasArn
  type: object
- description: ''
  name: kmsKeyArn
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-kms-key-schema.json
slug: ground-station-kms-key
source_filename: ground-station-kms-key-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-kms-key-schema.json\",\n  \"title\": \"KmsKey\",\n  \"description\": \"AWS Key Management Service (KMS) Key.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kmsAliasArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyAliasArn\"\n        },\n        {\n          \"description\": \"KMS Alias Arn.\"\n        }\n      ]\n    },\n    \"kmsKeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyArn\"\n        },\n        {\n          \"description\": \"KMS Key Arn.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-kms-key-schema.json
tags:
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: KmsKey
---
