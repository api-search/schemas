---
description: GetDataCatalogEncryptionSettingsResponse schema from Amazon Glue API
layout: schema
name: GetDataCatalogEncryptionSettingsResponse
properties_list:
- description: ''
  name: DataCatalogEncryptionSettings
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-data-catalog-encryption-settings-response-schema.json
slug: glue-get-data-catalog-encryption-settings-response
source_filename: glue-get-data-catalog-encryption-settings-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-data-catalog-encryption-settings-response-schema.json\",\n  \"title\": \"GetDataCatalogEncryptionSettingsResponse\",\n  \"description\": \"GetDataCatalogEncryptionSettingsResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DataCatalogEncryptionSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataCatalogEncryptionSettings\"\n        },\n        {\n          \"description\": \"The requested security configuration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-data-catalog-encryption-settings-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetDataCatalogEncryptionSettingsResponse
---
