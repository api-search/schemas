---
description: GetCatalogImportStatusResponse schema from Amazon Glue API
layout: schema
name: GetCatalogImportStatusResponse
properties_list:
- description: ''
  name: ImportStatus
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-catalog-import-status-response-schema.json
slug: glue-get-catalog-import-status-response
source_filename: glue-get-catalog-import-status-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-catalog-import-status-response-schema.json\",\n  \"title\": \"GetCatalogImportStatusResponse\",\n  \"description\": \"GetCatalogImportStatusResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ImportStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogImportStatus\"\n        },\n        {\n          \"description\": \"The status of the specified catalog migration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-catalog-import-status-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetCatalogImportStatusResponse
---
