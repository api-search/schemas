---
description: Defines an alternate key. This value is optional. A legacy data set might not have any alternate key defined but if those alternate keys definitions exist, provide them, as some applications will make use of them.
layout: schema
name: AlternateKey
properties_list:
- description: ''
  name: allowDuplicates
  type: object
- description: ''
  name: length
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: offset
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-alternate-key-schema.json
slug: amazon-mainframe-modernization-alternate-key
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-alternate-key-schema.json\",\n  \"title\": \"AlternateKey\",\n  \"description\": \"Defines an alternate key. This value is optional. A legacy data set might not have any alternate key defined but if those alternate keys definitions exist, provide them, as some applications will make use of them.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowDuplicates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Indicates whether the alternate key values are supposed to be unique for the given data set.\"\n        }\n      ]\n    },\n    \"length\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n   \
  \       \"description\": \"A strictly positive integer value representing the length of the alternate key.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the alternate key.\"\n        }\n      ]\n    },\n    \"offset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"A positive integer value representing the offset to mark the start of the alternate key part in the record byte array.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"length\",\n    \"offset\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-alternate-key-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: AlternateKey
---
