---
description: Defines a data set.
layout: schema
name: DataSet
properties_list:
- description: ''
  name: datasetName
  type: object
- description: ''
  name: datasetOrg
  type: object
- description: ''
  name: recordLength
  type: object
- description: ''
  name: relativePath
  type: object
- description: ''
  name: storageType
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-data-set-schema.json
slug: amazon-mainframe-modernization-data-set
source_filename: amazon-mainframe-modernization-data-set-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-data-set-schema.json\",\n  \"title\": \"DataSet\",\n  \"description\": \"Defines a data set.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"datasetName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The logical identifier for a specific data set (in mainframe format).\"\n        }\n      ]\n    },\n    \"datasetOrg\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetOrgAttributes\"\n        },\n        {\n          \"description\": \"The type of dataset. The only supported value is VSAM.\"\n        }\n      ]\n    },\n    \"recordLength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecordLength\"\
  \n        },\n        {\n          \"description\": \"The length of a record.\"\n        }\n      ]\n    },\n    \"relativePath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The relative location of the data set in the database or file system. \"\n        }\n      ]\n    },\n    \"storageType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The storage type of the data set: database or file system. For Micro Focus, database corresponds to datastore and file system corresponds to EFS/FSX. For Blu Age, there is no support of file system and database corresponds to Blusam. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"datasetName\",\n    \"datasetOrg\",\n    \"recordLength\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-data-set-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: DataSet
---
