---
description: GetDataSetDetailsResponse schema from AWS Mainframe Modernization API
layout: schema
name: GetDataSetDetailsResponse
properties_list:
- description: ''
  name: blocksize
  type: object
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
  name: lastReferencedTime
  type: object
- description: ''
  name: lastUpdatedTime
  type: object
- description: ''
  name: location
  type: object
- description: ''
  name: recordLength
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-get-data-set-details-response-schema.json
slug: amazon-mainframe-modernization-get-data-set-details-response
source_filename: amazon-mainframe-modernization-get-data-set-details-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-get-data-set-details-response-schema.json\",\n  \"title\": \"GetDataSetDetailsResponse\",\n  \"description\": \"GetDataSetDetailsResponse schema from AWS Mainframe Modernization API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"blocksize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The size of the block on disk. \"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The timestamp when the data set was created.\"\n        }\n      ]\n    },\n    \"dataSetName\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/String200\"\n        },\n        {\n          \"description\": \"The name of the data set.\"\n        }\n      ]\n    },\n    \"dataSetOrg\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetDetailOrgAttributes\"\n        },\n        {\n          \"description\": \"The type of data set. The only supported value is VSAM.\"\n        }\n      ]\n    },\n    \"lastReferencedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The last time the data set was referenced.\"\n        }\n      ]\n    },\n    \"lastUpdatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The last time the data set was updated.\"\n        }\n      ]\n    },\n    \"location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String2000\"\
  \n        },\n        {\n          \"description\": \"The location where the data set is stored.\"\n        }\n      ]\n    },\n    \"recordLength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The length of records in the data set.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"dataSetName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-get-data-set-details-response-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: GetDataSetDetailsResponse
---
