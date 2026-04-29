---
description: ListSchemaVersionsResponse schema from Amazon Glue API
layout: schema
name: ListSchemaVersionsResponse
properties_list:
- description: ''
  name: Schemas
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-list-schema-versions-response-schema.json
slug: glue-list-schema-versions-response
source_filename: glue-list-schema-versions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-schema-versions-response-schema.json\",\n  \"title\": \"ListSchemaVersionsResponse\",\n  \"description\": \"ListSchemaVersionsResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Schemas\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaVersionList\"\n        },\n        {\n          \"description\": \"An array of <code>SchemaVersionList</code> objects containing details of each schema version.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaRegistryTokenString\"\n        },\n        {\n          \"description\": \"A continuation token for paginating the returned list of tokens, returned if the current segment of the list is not the last.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-schema-versions-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: ListSchemaVersionsResponse
---
