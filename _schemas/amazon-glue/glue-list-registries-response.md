---
description: ListRegistriesResponse schema from Amazon Glue API
layout: schema
name: ListRegistriesResponse
properties_list:
- description: ''
  name: Registries
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-list-registries-response-schema.json
slug: glue-list-registries-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-registries-response-schema.json\",\n  \"title\": \"ListRegistriesResponse\",\n  \"description\": \"ListRegistriesResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Registries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegistryListDefinition\"\n        },\n        {\n          \"description\": \"An array of <code>RegistryDetailedListItem</code> objects containing minimal details of each registry.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaRegistryTokenString\"\n        },\n        {\n          \"description\": \"A continuation token for paginating the returned list of tokens, returned if the current segment of the list is not the last.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-registries-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: ListRegistriesResponse
---
