---
description: Contains a list of values defining partitions.
layout: schema
name: PartitionValueList
properties_list:
- description: ''
  name: Values
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-partition-value-list-schema.json
slug: glue-partition-value-list
source_filename: glue-partition-value-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-partition-value-list-schema.json\",\n  \"title\": \"PartitionValueList\",\n  \"description\": \"Contains a list of values defining partitions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Values\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ValueStringList\"\n        },\n        {\n          \"description\": \"The list of values.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Values\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-partition-value-list-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: PartitionValueList
---
