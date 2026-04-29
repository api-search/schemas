---
description: The supported properties for a PO type data set.
layout: schema
name: PoAttributes
properties_list:
- description: ''
  name: encoding
  type: object
- description: ''
  name: format
  type: object
- description: ''
  name: memberFileExtensions
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-po-attributes-schema.json
slug: amazon-mainframe-modernization-po-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-po-attributes-schema.json\",\n  \"title\": \"PoAttributes\",\n  \"description\": \"The supported properties for a PO type data set.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"encoding\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The character set encoding of the data set.\"\n        }\n      ]\n    },\n    \"format\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The format of the data set records.\"\n        }\n      ]\n    },\n    \"memberFileExtensions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String20List\"\n       \
  \ },\n        {\n          \"description\": \"An array containing one or more filename extensions, allowing you to specify which files to be included as PDS member.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"format\",\n    \"memberFileExtensions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-po-attributes-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: PoAttributes
---
