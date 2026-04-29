---
description: A Microsoft Smooth Streaming (MSS) encryption configuration.
layout: schema
name: MssEncryption
properties_list:
- description: ''
  name: SpekeKeyProvider
  type: object
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-mss-encryption-schema.json
slug: mediapackage-api-mss-encryption
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-mss-encryption-schema.json\",\n  \"title\": \"MssEncryption\",\n  \"description\": \"A Microsoft Smooth Streaming (MSS) encryption configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SpekeKeyProvider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SpekeKeyProvider\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"spekeKeyProvider\"\n          }\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SpekeKeyProvider\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-mss-encryption-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: MssEncryption
---
