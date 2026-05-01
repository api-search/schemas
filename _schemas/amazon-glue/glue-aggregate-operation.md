---
description: Specifies the set of parameters needed to perform aggregation in the aggregate transform.
layout: schema
name: AggregateOperation
properties_list:
- description: ''
  name: Column
  type: object
- description: ''
  name: AggFunc
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-aggregate-operation-schema.json
slug: glue-aggregate-operation
source_filename: glue-aggregate-operation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-aggregate-operation-schema.json\",\n  \"title\": \"AggregateOperation\",\n  \"description\": \"Specifies the set of parameters needed to perform aggregation in the aggregate transform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Column\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnclosedInStringProperties\"\n        },\n        {\n          \"description\": \"Specifies the column on the data set on which the aggregation function will be applied.\"\n        }\n      ]\n    },\n    \"AggFunc\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggFunction\"\n        },\n        {\n          \"description\": \"<p>Specifies the aggregation function to apply.</p> <p>Possible aggregation functions include: avg countDistinct, count, first,\
  \ last, kurtosis, max, min, skewness, stddev_samp, stddev_pop, sum, sumDistinct, var_samp, var_pop</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Column\",\n    \"AggFunc\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-aggregate-operation-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: AggregateOperation
---
