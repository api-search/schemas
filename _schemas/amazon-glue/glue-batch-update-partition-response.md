---
description: BatchUpdatePartitionResponse schema from Amazon Glue API
layout: schema
name: BatchUpdatePartitionResponse
properties_list:
- description: ''
  name: Errors
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-batch-update-partition-response-schema.json
slug: glue-batch-update-partition-response
source_filename: glue-batch-update-partition-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-update-partition-response-schema.json\",\n  \"title\": \"BatchUpdatePartitionResponse\",\n  \"description\": \"BatchUpdatePartitionResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Errors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchUpdatePartitionFailureList\"\n        },\n        {\n          \"description\": \"The errors encountered when trying to update the requested partitions. A list of <code>BatchUpdatePartitionFailureEntry</code> objects.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-update-partition-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: BatchUpdatePartitionResponse
---
