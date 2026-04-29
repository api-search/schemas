---
description: Specifies a transform that groups rows by chosen fields and computes the aggregated value by specified function.
layout: schema
name: Aggregate
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Inputs
  type: object
- description: ''
  name: Groups
  type: object
- description: ''
  name: Aggs
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-aggregate-schema.json
slug: glue-aggregate
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-aggregate-schema.json\",\n  \"title\": \"Aggregate\",\n  \"description\": \"Specifies a transform that groups rows by chosen fields and computes the aggregated value by specified function.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeName\"\n        },\n        {\n          \"description\": \"The name of the transform node.\"\n        }\n      ]\n    },\n    \"Inputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OneInput\"\n        },\n        {\n          \"description\": \"Specifies the fields and rows to use as inputs for the aggregate transform.\"\n        }\n      ]\n    },\n    \"Groups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GlueStudioPathList\"\
  \n        },\n        {\n          \"description\": \"Specifies the fields to group by.\"\n        }\n      ]\n    },\n    \"Aggs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregateOperations\"\n        },\n        {\n          \"description\": \"Specifies the aggregate functions to be performed on specified fields. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"Inputs\",\n    \"Groups\",\n    \"Aggs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-aggregate-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: Aggregate
---
