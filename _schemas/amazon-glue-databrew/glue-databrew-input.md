---
description: Represents information on how DataBrew can find data, in either the Glue Data Catalog or Amazon S3.
layout: schema
name: Input
properties_list:
- description: ''
  name: S3InputDefinition
  type: object
- description: ''
  name: DataCatalogInputDefinition
  type: object
- description: ''
  name: DatabaseInputDefinition
  type: object
- description: ''
  name: Metadata
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-input-schema.json
slug: glue-databrew-input
source_filename: glue-databrew-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-input-schema.json\",\n  \"title\": \"Input\",\n  \"description\": \"Represents information on how DataBrew can find data, in either the Glue Data Catalog or Amazon S3.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3InputDefinition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Location\"\n        },\n        {\n          \"description\": \"The Amazon S3 location where the data is stored.\"\n        }\n      ]\n    },\n    \"DataCatalogInputDefinition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataCatalogInputDefinition\"\n        },\n        {\n          \"description\": \"The Glue Data Catalog parameters for the data.\"\n        }\n      ]\n    },\n    \"DatabaseInputDefinition\": {\n      \"allOf\":\
  \ [\n        {\n          \"$ref\": \"#/components/schemas/DatabaseInputDefinition\"\n        },\n        {\n          \"description\": \"Connection information for dataset input files stored in a database.\"\n        }\n      ]\n    },\n    \"Metadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Metadata\"\n        },\n        {\n          \"description\": \"Contains additional resource information needed for specific datasets.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-input-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: Input
---
