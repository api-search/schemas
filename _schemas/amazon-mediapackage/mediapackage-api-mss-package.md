---
description: A Microsoft Smooth Streaming (MSS) packaging configuration.
layout: schema
name: MssPackage
properties_list:
- description: ''
  name: Encryption
  type: object
- description: ''
  name: ManifestWindowSeconds
  type: object
- description: ''
  name: SegmentDurationSeconds
  type: object
- description: ''
  name: StreamSelection
  type: object
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-mss-package-schema.json
slug: mediapackage-api-mss-package
source_filename: mediapackage-api-mss-package-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-mss-package-schema.json\",\n  \"title\": \"MssPackage\",\n  \"description\": \"A Microsoft Smooth Streaming (MSS) packaging configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Encryption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MssEncryption\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encryption\"\n          }\n        }\n      ]\n    },\n    \"ManifestWindowSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"manifestWindowSeconds\"\n          },\n          \"description\": \"The time window (in seconds) contained in each manifest.\"\n        }\n      ]\n    },\n    \"SegmentDurationSeconds\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentDurationSeconds\"\n          },\n          \"description\": \"The duration (in seconds) of each segment.\"\n        }\n      ]\n    },\n    \"StreamSelection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamSelection\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"streamSelection\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-mss-package-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: MssPackage
---
