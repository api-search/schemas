---
description: GetConnectionRequest schema from Amazon Glue API
layout: schema
name: GetConnectionRequest
properties_list:
- description: ''
  name: CatalogId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: HidePassword
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-connection-request-schema.json
slug: glue-get-connection-request
source_filename: glue-get-connection-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-connection-request-schema.json\",\n  \"title\": \"GetConnectionRequest\",\n  \"description\": \"GetConnectionRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CatalogId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogIdString\"\n        },\n        {\n          \"description\": \"The ID of the Data Catalog in which the connection resides. If none is provided, the Amazon Web Services account ID is used by default.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the connection definition to retrieve.\"\n        }\n      ]\n    },\n    \"HidePassword\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Allows you to retrieve the connection metadata without returning the password. For instance, the Glue console uses this flag to retrieve the connection, and does not display the password. Set this parameter when the caller might not have permission to use the KMS key to decrypt the password, but it does have permission to access the rest of the connection properties.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-connection-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetConnectionRequest
---
