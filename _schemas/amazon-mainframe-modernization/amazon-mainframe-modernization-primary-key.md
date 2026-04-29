---
description: The primary key for a KSDS data set.
layout: schema
name: PrimaryKey
properties_list:
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
schema_file: json-schema/amazon-mainframe-modernization-primary-key-schema.json
slug: amazon-mainframe-modernization-primary-key
source_filename: amazon-mainframe-modernization-primary-key-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-primary-key-schema.json\",\n  \"title\": \"PrimaryKey\",\n  \"description\": \"The primary key for a KSDS data set.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"length\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"A strictly positive integer value representing the length of the primary key. \"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A name for the Primary Key.\"\n        }\n      ]\n    },\n    \"offset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n      \
  \  {\n          \"description\": \"A positive integer value representing the offset to mark the start of the primary key in the record byte array.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"length\",\n    \"offset\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-primary-key-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: PrimaryKey
---
