---
description: QuerySchemaVersionMetadataResponse schema from Amazon Glue API
layout: schema
name: QuerySchemaVersionMetadataResponse
properties_list:
- description: ''
  name: MetadataInfoMap
  type: object
- description: ''
  name: SchemaVersionId
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-query-schema-version-metadata-response-schema.json
slug: glue-query-schema-version-metadata-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-query-schema-version-metadata-response-schema.json\",\n  \"title\": \"QuerySchemaVersionMetadataResponse\",\n  \"description\": \"QuerySchemaVersionMetadataResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MetadataInfoMap\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetadataInfoMap\"\n        },\n        {\n          \"description\": \"A map of a metadata key and associated values.\"\n        }\n      ]\n    },\n    \"SchemaVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaVersionIdString\"\n        },\n        {\n          \"description\": \"The unique version ID of the schema version.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n         \
  \ \"$ref\": \"#/components/schemas/SchemaRegistryTokenString\"\n        },\n        {\n          \"description\": \"A continuation token for paginating the returned list of tokens, returned if the current segment of the list is not the last.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-query-schema-version-metadata-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: QuerySchemaVersionMetadataResponse
---
