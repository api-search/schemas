---
description: GetTableVersionsResponse schema from Amazon Glue API
layout: schema
name: GetTableVersionsResponse
properties_list:
- description: ''
  name: TableVersions
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-table-versions-response-schema.json
slug: glue-get-table-versions-response
source_filename: glue-get-table-versions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-table-versions-response-schema.json\",\n  \"title\": \"GetTableVersionsResponse\",\n  \"description\": \"GetTableVersionsResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GetTableVersionsList\"\n        },\n        {\n          \"description\": \"A list of strings identifying available versions of the specified table.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"A continuation token, if the list of available versions does not include the last one.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-table-versions-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetTableVersionsResponse
---
