---
description: Identifies one or more data sets you want to import with the <a>CreateDataSetImportTask</a> operation.
layout: schema
name: DataSetImportConfig
properties_list:
- description: ''
  name: dataSets
  type: object
- description: ''
  name: s3Location
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-data-set-import-config-schema.json
slug: amazon-mainframe-modernization-data-set-import-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-data-set-import-config-schema.json\",\n  \"title\": \"DataSetImportConfig\",\n  \"description\": \"Identifies one or more data sets you want to import with the <a>CreateDataSetImportTask</a> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dataSets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSetImportList\"\n        },\n        {\n          \"description\": \"The data sets.\"\n        }\n      ]\n    },\n    \"s3Location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String2000\"\n        },\n        {\n          \"description\": \"The Amazon S3 location of the data sets.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-data-set-import-config-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: DataSetImportConfig
---
