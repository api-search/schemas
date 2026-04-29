---
description: QuerySchemaVersionMetadataInput schema from Amazon Glue API
layout: schema
name: QuerySchemaVersionMetadataInput
properties_list:
- description: ''
  name: SchemaId
  type: object
- description: ''
  name: SchemaVersionNumber
  type: object
- description: ''
  name: SchemaVersionId
  type: object
- description: ''
  name: MetadataList
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-query-schema-version-metadata-input-schema.json
slug: glue-query-schema-version-metadata-input
source_filename: glue-query-schema-version-metadata-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-query-schema-version-metadata-input-schema.json\",\n  \"title\": \"QuerySchemaVersionMetadataInput\",\n  \"description\": \"QuerySchemaVersionMetadataInput schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SchemaId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaId\"\n        },\n        {\n          \"description\": \"A wrapper structure that may contain the schema name and Amazon Resource Name (ARN).\"\n        }\n      ]\n    },\n    \"SchemaVersionNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaVersionNumber\"\n        },\n        {\n          \"description\": \"The version number of the schema.\"\n        }\n      ]\n    },\n    \"SchemaVersionId\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/SchemaVersionIdString\"\n        },\n        {\n          \"description\": \"The unique version ID of the schema version.\"\n        }\n      ]\n    },\n    \"MetadataList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetadataList\"\n        },\n        {\n          \"description\": \"Search key-value pairs for metadata, if they are not provided all the metadata information will be fetched.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QuerySchemaVersionMetadataMaxResults\"\n        },\n        {\n          \"description\": \"Maximum number of results required per page. If the value is not supplied, this will be defaulted to 25 per page.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaRegistryTokenString\"\n        },\n        {\n          \"description\"\
  : \"A continuation token, if this is a continuation call.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-query-schema-version-metadata-input-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: QuerySchemaVersionMetadataInput
---
