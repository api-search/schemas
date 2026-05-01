---
description: GetPartitionIndexesResponse schema from Amazon Glue API
layout: schema
name: GetPartitionIndexesResponse
properties_list:
- description: ''
  name: PartitionIndexDescriptorList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-partition-indexes-response-schema.json
slug: glue-get-partition-indexes-response
source_filename: glue-get-partition-indexes-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-partition-indexes-response-schema.json\",\n  \"title\": \"GetPartitionIndexesResponse\",\n  \"description\": \"GetPartitionIndexesResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PartitionIndexDescriptorList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PartitionIndexDescriptorList\"\n        },\n        {\n          \"description\": \"A list of index descriptors.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"A continuation token, present if the current list segment is not the last.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-partition-indexes-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetPartitionIndexesResponse
---
