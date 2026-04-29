---
description: Identifies a specific data set to import from an external location.
layout: schema
name: DataSetImportItem
properties_list:
- description: ''
  name: dataSet
  type: object
- description: ''
  name: externalLocation
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-data-set-import-item-schema.json
slug: amazon-mainframe-modernization-data-set-import-item
source_filename: amazon-mainframe-modernization-data-set-import-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-data-set-import-item-schema.json\",\n  \"title\": \"DataSetImportItem\",\n  \"description\": \"Identifies a specific data set to import from an external location.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dataSet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSet\"\n        },\n        {\n          \"description\": \"The data set.\"\n        }\n      ]\n    },\n    \"externalLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExternalLocation\"\n        },\n        {\n          \"description\": \"The location of the data set.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"dataSet\",\n    \"externalLocation\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-data-set-import-item-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: DataSetImportItem
---
