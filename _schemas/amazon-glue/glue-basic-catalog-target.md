---
description: Specifies a target that uses a Glue Data Catalog table.
layout: schema
name: BasicCatalogTarget
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Inputs
  type: object
- description: ''
  name: Database
  type: object
- description: ''
  name: Table
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-basic-catalog-target-schema.json
slug: glue-basic-catalog-target
source_filename: glue-basic-catalog-target-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-basic-catalog-target-schema.json\",\n  \"title\": \"BasicCatalogTarget\",\n  \"description\": \"Specifies a target that uses a Glue Data Catalog table.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeName\"\n        },\n        {\n          \"description\": \"The name of your data target.\"\n        }\n      ]\n    },\n    \"Inputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OneInput\"\n        },\n        {\n          \"description\": \"The nodes that are inputs to the data target.\"\n        }\n      ]\n    },\n    \"Database\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnclosedInStringProperty\"\n        },\n        {\n          \"description\"\
  : \"The database that contains the table you want to use as the target. This database must already exist in the Data Catalog.\"\n        }\n      ]\n    },\n    \"Table\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnclosedInStringProperty\"\n        },\n        {\n          \"description\": \"The table that defines the schema of your output data. This table must already exist in the Data Catalog.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"Inputs\",\n    \"Database\",\n    \"Table\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-basic-catalog-target-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: BasicCatalogTarget
---
