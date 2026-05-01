---
description: GetDatabasesResponse schema from Amazon Glue API
layout: schema
name: GetDatabasesResponse
properties_list:
- description: ''
  name: DatabaseList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-databases-response-schema.json
slug: glue-get-databases-response
source_filename: glue-get-databases-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-databases-response-schema.json\",\n  \"title\": \"GetDatabasesResponse\",\n  \"description\": \"GetDatabasesResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DatabaseList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatabaseList\"\n        },\n        {\n          \"description\": \"A list of <code>Database</code> objects from the specified catalog.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"A continuation token for paginating the returned list of tokens, returned if the current segment of the list is not the last.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DatabaseList\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-databases-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetDatabasesResponse
---
