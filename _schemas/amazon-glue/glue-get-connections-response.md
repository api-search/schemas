---
description: GetConnectionsResponse schema from Amazon Glue API
layout: schema
name: GetConnectionsResponse
properties_list:
- description: ''
  name: ConnectionList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-connections-response-schema.json
slug: glue-get-connections-response
source_filename: glue-get-connections-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-connections-response-schema.json\",\n  \"title\": \"GetConnectionsResponse\",\n  \"description\": \"GetConnectionsResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConnectionList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionList\"\n        },\n        {\n          \"description\": \"A list of requested connection definitions.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"A continuation token, if the list of connections returned does not include the last of the filtered connections.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-connections-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetConnectionsResponse
---
