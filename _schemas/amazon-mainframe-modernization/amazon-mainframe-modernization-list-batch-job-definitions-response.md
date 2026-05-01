---
description: ListBatchJobDefinitionsResponse schema from AWS Mainframe Modernization API
layout: schema
name: ListBatchJobDefinitionsResponse
properties_list:
- description: ''
  name: batchJobDefinitions
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-list-batch-job-definitions-response-schema.json
slug: amazon-mainframe-modernization-list-batch-job-definitions-response
source_filename: amazon-mainframe-modernization-list-batch-job-definitions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-list-batch-job-definitions-response-schema.json\",\n  \"title\": \"ListBatchJobDefinitionsResponse\",\n  \"description\": \"ListBatchJobDefinitionsResponse schema from AWS Mainframe Modernization API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"batchJobDefinitions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchJobDefinitions\"\n        },\n        {\n          \"description\": \"The list of batch job definitions.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"If there are more items to return, this contains a token that is passed to a subsequent call to this operation\
  \ to retrieve the next set of items.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"batchJobDefinitions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-list-batch-job-definitions-response-schema.json
tags:
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: ListBatchJobDefinitionsResponse
---
