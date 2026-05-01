---
description: CreateConnectionRequest schema from Amazon Glue API
layout: schema
name: CreateConnectionRequest
properties_list:
- description: ''
  name: CatalogId
  type: object
- description: ''
  name: ConnectionInput
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-create-connection-request-schema.json
slug: glue-create-connection-request
source_filename: glue-create-connection-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-connection-request-schema.json\",\n  \"title\": \"CreateConnectionRequest\",\n  \"description\": \"CreateConnectionRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CatalogId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogIdString\"\n        },\n        {\n          \"description\": \"The ID of the Data Catalog in which to create the connection. If none is provided, the Amazon Web Services account ID is used by default.\"\n        }\n      ]\n    },\n    \"ConnectionInput\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionInput\"\n        },\n        {\n          \"description\": \"A <code>ConnectionInput</code> object defining the connection to create.\"\n        }\n      ]\n\
  \    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagsMap\"\n        },\n        {\n          \"description\": \"The tags you assign to the connection.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConnectionInput\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-connection-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: CreateConnectionRequest
---
