---
description: GetPartitionsResponse schema from Amazon Glue API
layout: schema
name: GetPartitionsResponse
properties_list:
- description: ''
  name: Partitions
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-partitions-response-schema.json
slug: glue-get-partitions-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-partitions-response-schema.json\",\n  \"title\": \"GetPartitionsResponse\",\n  \"description\": \"GetPartitionsResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Partitions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PartitionList\"\n        },\n        {\n          \"description\": \"A list of requested partitions.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"A continuation token, if the returned list of partitions does not include the last one.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-partitions-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetPartitionsResponse
---
