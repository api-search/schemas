---
description: The attributes of a VSAM type data set.
layout: schema
name: VsamAttributes
properties_list:
- description: ''
  name: alternateKeys
  type: object
- description: ''
  name: compressed
  type: object
- description: ''
  name: encoding
  type: object
- description: ''
  name: format
  type: object
- description: ''
  name: primaryKey
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-vsam-attributes-schema.json
slug: amazon-mainframe-modernization-vsam-attributes
source_filename: amazon-mainframe-modernization-vsam-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-vsam-attributes-schema.json\",\n  \"title\": \"VsamAttributes\",\n  \"description\": \"The attributes of a VSAM type data set.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"alternateKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlternateKeyList\"\n        },\n        {\n          \"description\": \"The alternate key definitions, if any. A legacy dataset might not have any alternate key defined, but if those alternate keys definitions exist, provide them as some applications will make use of them.\"\n        }\n      ]\n    },\n    \"compressed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Indicates whether indexes\
  \ for this dataset are stored as compressed values. If you have a large data set (typically &gt; 100 Mb), consider setting this flag to True.\"\n        }\n      ]\n    },\n    \"encoding\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The character set used by the data set. Can be ASCII, EBCDIC, or unknown.\"\n        }\n      ]\n    },\n    \"format\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The record format of the data set.\"\n        }\n      ]\n    },\n    \"primaryKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrimaryKey\"\n        },\n        {\n          \"description\": \"The primary key of the data set.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"format\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-vsam-attributes-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: VsamAttributes
---
