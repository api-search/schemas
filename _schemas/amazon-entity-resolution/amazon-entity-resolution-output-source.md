---
description: A list of <code>OutputAttribute</code> objects, each of which have the fields Name and Hashed. Each of these objects selects a column to be included in the output table, and whether the values of the column should be hashed.
layout: schema
name: OutputSource
properties_list:
- description: ''
  name: KMSArn
  type: object
- description: ''
  name: applyNormalization
  type: object
- description: ''
  name: output
  type: object
- description: ''
  name: outputS3Path
  type: object
provider_name: Amazon Entity Resolution
provider_slug: amazon-entity-resolution
schema_file: json-schema/amazon-entity-resolution-output-source-schema.json
slug: amazon-entity-resolution-output-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-output-source-schema.json\",\n  \"title\": \"OutputSource\",\n  \"description\": \"A list of <code>OutputAttribute</code> objects, each of which have the fields Name and Hashed. Each of these objects selects a column to be included in the output table, and whether the values of the column should be hashed.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"KMSArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KMSArn\"\n        },\n        {\n          \"description\": \"Customer KMS ARN for encryption at rest. If not provided, system will use an Entity Resolution managed KMS key.\"\n        }\n      ]\n    },\n    \"applyNormalization\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n      \
  \  },\n        {\n          \"description\": \"Normalizes the attributes defined in the schema in the input data. For example, if an attribute has an <code>AttributeType</code> of <code>PHONE_NUMBER</code>, and the data in the input table is in a format of 1234567890, Entity Resolution will normalize this field in the output to (123)-456-7890.\"\n        }\n      ]\n    },\n    \"output\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputSourceOutputList\"\n        },\n        {\n          \"description\": \"A list of <code>OutputAttribute</code> objects, each of which have the fields Name and Hashed. Each of these objects selects a column to be included in the output table, and whether the values of the column should be hashed.\"\n        }\n      ]\n    },\n    \"outputS3Path\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputSourceOutputS3PathString\"\n        },\n        {\n          \"description\": \"The S3 path\
  \ to which Entity Resolution will write the output table.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"output\",\n    \"outputS3Path\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-output-source-schema.json
tags:
- Amazon Web Services
- AWS
- Data Integration
- Data Matching
- Entity Resolution
- Machine Learning
title: OutputSource
---
