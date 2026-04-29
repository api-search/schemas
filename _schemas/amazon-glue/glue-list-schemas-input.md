---
description: ListSchemasInput schema from Amazon Glue API
layout: schema
name: ListSchemasInput
properties_list:
- description: ''
  name: RegistryId
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-list-schemas-input-schema.json
slug: glue-list-schemas-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-schemas-input-schema.json\",\n  \"title\": \"ListSchemasInput\",\n  \"description\": \"ListSchemasInput schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RegistryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegistryId\"\n        },\n        {\n          \"description\": \"A wrapper structure that may contain the registry name and Amazon Resource Name (ARN).\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResultsNumber\"\n        },\n        {\n          \"description\": \"Maximum number of results required per page. If the value is not supplied, this will be defaulted to 25 per page.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaRegistryTokenString\"\n        },\n        {\n          \"description\": \"A continuation token, if this is a continuation call.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-schemas-input-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: ListSchemasInput
---
