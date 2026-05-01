---
description: The supported properties for a PS type data set.
layout: schema
name: PsDetailAttributes
properties_list:
- description: ''
  name: encoding
  type: object
- description: ''
  name: format
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-ps-detail-attributes-schema.json
slug: amazon-mainframe-modernization-ps-detail-attributes
source_filename: amazon-mainframe-modernization-ps-detail-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-ps-detail-attributes-schema.json\",\n  \"title\": \"PsDetailAttributes\",\n  \"description\": \"The supported properties for a PS type data set.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"encoding\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The character set encoding of the data set.\"\n        }\n      ]\n    },\n    \"format\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The format of the data set records.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"encoding\",\n    \"format\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-ps-detail-attributes-schema.json
tags:
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: PsDetailAttributes
---
