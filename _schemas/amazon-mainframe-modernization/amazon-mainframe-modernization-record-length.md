---
description: The length of the records in the data set.
layout: schema
name: RecordLength
properties_list:
- description: ''
  name: max
  type: object
- description: ''
  name: min
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-record-length-schema.json
slug: amazon-mainframe-modernization-record-length
source_filename: amazon-mainframe-modernization-record-length-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-record-length-schema.json\",\n  \"title\": \"RecordLength\",\n  \"description\": \"The length of the records in the data set.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"max\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The maximum record length. In case of fixed, both minimum and maximum are the same.\"\n        }\n      ]\n    },\n    \"min\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The minimum record length of a record.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"max\",\n    \"min\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-record-length-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: RecordLength
---
