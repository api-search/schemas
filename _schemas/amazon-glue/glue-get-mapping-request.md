---
description: GetMappingRequest schema from Amazon Glue API
layout: schema
name: GetMappingRequest
properties_list:
- description: ''
  name: Source
  type: object
- description: ''
  name: Sinks
  type: object
- description: ''
  name: Location
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-mapping-request-schema.json
slug: glue-get-mapping-request
source_filename: glue-get-mapping-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-mapping-request-schema.json\",\n  \"title\": \"GetMappingRequest\",\n  \"description\": \"GetMappingRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogEntry\"\n        },\n        {\n          \"description\": \"Specifies the source table.\"\n        }\n      ]\n    },\n    \"Sinks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogEntries\"\n        },\n        {\n          \"description\": \"A list of target tables.\"\n        }\n      ]\n    },\n    \"Location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Location\"\n        },\n        {\n          \"description\": \"Parameters for the mapping.\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Source\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-mapping-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetMappingRequest
---
