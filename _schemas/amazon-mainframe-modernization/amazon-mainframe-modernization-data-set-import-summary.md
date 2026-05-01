---
description: Represents a summary of data set imports.
layout: schema
name: DataSetImportSummary
properties_list:
- description: ''
  name: failed
  type: object
- description: ''
  name: inProgress
  type: object
- description: ''
  name: pending
  type: object
- description: ''
  name: succeeded
  type: object
- description: ''
  name: total
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-data-set-import-summary-schema.json
slug: amazon-mainframe-modernization-data-set-import-summary
source_filename: amazon-mainframe-modernization-data-set-import-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-data-set-import-summary-schema.json\",\n  \"title\": \"DataSetImportSummary\",\n  \"description\": \"Represents a summary of data set imports.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"failed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of data set imports that have failed.\"\n        }\n      ]\n    },\n    \"inProgress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of data set imports that are in progress.\"\n        }\n      ]\n    },\n    \"pending\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\
  \n        },\n        {\n          \"description\": \"The number of data set imports that are pending.\"\n        }\n      ]\n    },\n    \"succeeded\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of data set imports that have succeeded.\"\n        }\n      ]\n    },\n    \"total\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The total number of data set imports.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"failed\",\n    \"inProgress\",\n    \"pending\",\n    \"succeeded\",\n    \"total\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-data-set-import-summary-schema.json
tags:
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: DataSetImportSummary
---
