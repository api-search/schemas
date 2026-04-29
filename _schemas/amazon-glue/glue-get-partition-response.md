---
description: GetPartitionResponse schema from Amazon Glue API
layout: schema
name: GetPartitionResponse
properties_list:
- description: ''
  name: Partition
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-partition-response-schema.json
slug: glue-get-partition-response
source_filename: glue-get-partition-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-partition-response-schema.json\",\n  \"title\": \"GetPartitionResponse\",\n  \"description\": \"GetPartitionResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Partition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Partition\"\n        },\n        {\n          \"description\": \"The requested information, in the form of a <code>Partition</code> object.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-partition-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetPartitionResponse
---
