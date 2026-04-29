---
description: A subset of the possible data set attributes.
layout: schema
name: DataSetSummary
properties_list:
- description: ''
  name: creationTime
  type: object
- description: ''
  name: dataSetName
  type: object
- description: ''
  name: dataSetOrg
  type: object
- description: ''
  name: format
  type: object
- description: ''
  name: lastReferencedTime
  type: object
- description: ''
  name: lastUpdatedTime
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-data-set-summary-schema.json
slug: amazon-mainframe-modernization-data-set-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-data-set-summary-schema.json\",\n  \"title\": \"DataSetSummary\",\n  \"description\": \"A subset of the possible data set attributes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The timestamp when the data set was created.\"\n        }\n      ]\n    },\n    \"dataSetName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String200\"\n        },\n        {\n          \"description\": \"The name of the data set.\"\n        }\n      ]\n    },\n    \"dataSetOrg\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String20\"\n        },\n \
  \       {\n          \"description\": \"The type of data set. The only supported value is VSAM.\"\n        }\n      ]\n    },\n    \"format\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String20\"\n        },\n        {\n          \"description\": \"The format of the data set. \"\n        }\n      ]\n    },\n    \"lastReferencedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The last time the data set was referenced.\"\n        }\n      ]\n    },\n    \"lastUpdatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The last time the data set was updated.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"dataSetName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-data-set-summary-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: DataSetSummary
---
