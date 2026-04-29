---
description: PutDataCatalogEncryptionSettingsRequest schema from Amazon Glue API
layout: schema
name: PutDataCatalogEncryptionSettingsRequest
properties_list:
- description: ''
  name: CatalogId
  type: object
- description: ''
  name: DataCatalogEncryptionSettings
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-put-data-catalog-encryption-settings-request-schema.json
slug: glue-put-data-catalog-encryption-settings-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-put-data-catalog-encryption-settings-request-schema.json\",\n  \"title\": \"PutDataCatalogEncryptionSettingsRequest\",\n  \"description\": \"PutDataCatalogEncryptionSettingsRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CatalogId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogIdString\"\n        },\n        {\n          \"description\": \"The ID of the Data Catalog to set the security configuration for. If none is provided, the Amazon Web Services account ID is used by default.\"\n        }\n      ]\n    },\n    \"DataCatalogEncryptionSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataCatalogEncryptionSettings\"\n        },\n        {\n          \"description\": \"The security\
  \ configuration to set.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DataCatalogEncryptionSettings\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-put-data-catalog-encryption-settings-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: PutDataCatalogEncryptionSettingsRequest
---
