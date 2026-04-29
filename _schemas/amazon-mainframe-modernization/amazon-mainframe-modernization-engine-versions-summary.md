---
description: A subset of information about the engine version for a specific application.
layout: schema
name: EngineVersionsSummary
properties_list:
- description: ''
  name: engineType
  type: object
- description: ''
  name: engineVersion
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-engine-versions-summary-schema.json
slug: amazon-mainframe-modernization-engine-versions-summary
source_filename: amazon-mainframe-modernization-engine-versions-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-engine-versions-summary-schema.json\",\n  \"title\": \"EngineVersionsSummary\",\n  \"description\": \"A subset of information about the engine version for a specific application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"engineType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The type of target platform for the application.\"\n        }\n      ]\n    },\n    \"engineVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The version of the engine type used by the application.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"engineType\",\n    \"\
  engineVersion\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-engine-versions-summary-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: EngineVersionsSummary
---
