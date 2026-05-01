---
description: Specifies a transform that maps data property keys in the data source to data property keys in the data target. You can rename keys, modify the data types for keys, and choose which keys to drop from the dataset.
layout: schema
name: ApplyMapping
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Inputs
  type: object
- description: ''
  name: Mapping
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-apply-mapping-schema.json
slug: glue-apply-mapping
source_filename: glue-apply-mapping-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-apply-mapping-schema.json\",\n  \"title\": \"ApplyMapping\",\n  \"description\": \"Specifies a transform that maps data property keys in the data source to data property keys in the data target. You can rename keys, modify the data types for keys, and choose which keys to drop from the dataset.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeName\"\n        },\n        {\n          \"description\": \"The name of the transform node.\"\n        }\n      ]\n    },\n    \"Inputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OneInput\"\n        },\n        {\n          \"description\": \"The data inputs identified by their node names.\"\n        }\n      ]\n    },\n    \"Mapping\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mappings\"\n        },\n        {\n          \"description\": \"Specifies the mapping of data property keys in the data source to data property keys in the data target.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"Inputs\",\n    \"Mapping\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-apply-mapping-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: ApplyMapping
---
