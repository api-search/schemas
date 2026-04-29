---
description: GetDataCatalogEncryptionSettingsRequest schema from Amazon Glue API
layout: schema
name: GetDataCatalogEncryptionSettingsRequest
properties_list:
- description: ''
  name: CatalogId
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-data-catalog-encryption-settings-request-schema.json
slug: glue-get-data-catalog-encryption-settings-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-data-catalog-encryption-settings-request-schema.json\",\n  \"title\": \"GetDataCatalogEncryptionSettingsRequest\",\n  \"description\": \"GetDataCatalogEncryptionSettingsRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CatalogId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogIdString\"\n        },\n        {\n          \"description\": \"The ID of the Data Catalog to retrieve the security configuration for. If none is provided, the Amazon Web Services account ID is used by default.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-data-catalog-encryption-settings-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetDataCatalogEncryptionSettingsRequest
---
