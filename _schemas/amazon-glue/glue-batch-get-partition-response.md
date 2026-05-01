---
description: BatchGetPartitionResponse schema from Amazon Glue API
layout: schema
name: BatchGetPartitionResponse
properties_list:
- description: ''
  name: Partitions
  type: object
- description: ''
  name: UnprocessedKeys
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-batch-get-partition-response-schema.json
slug: glue-batch-get-partition-response
source_filename: glue-batch-get-partition-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-partition-response-schema.json\",\n  \"title\": \"BatchGetPartitionResponse\",\n  \"description\": \"BatchGetPartitionResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Partitions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PartitionList\"\n        },\n        {\n          \"description\": \"A list of the requested partitions.\"\n        }\n      ]\n    },\n    \"UnprocessedKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchGetPartitionValueList\"\n        },\n        {\n          \"description\": \"A list of the partition values in the request for which partitions were not returned.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-partition-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: BatchGetPartitionResponse
---
