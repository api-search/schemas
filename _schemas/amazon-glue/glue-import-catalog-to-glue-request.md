---
description: ImportCatalogToGlueRequest schema from Amazon Glue API
layout: schema
name: ImportCatalogToGlueRequest
properties_list:
- description: ''
  name: CatalogId
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-import-catalog-to-glue-request-schema.json
slug: glue-import-catalog-to-glue-request
source_filename: glue-import-catalog-to-glue-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-import-catalog-to-glue-request-schema.json\",\n  \"title\": \"ImportCatalogToGlueRequest\",\n  \"description\": \"ImportCatalogToGlueRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CatalogId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogIdString\"\n        },\n        {\n          \"description\": \"The ID of the catalog to import. Currently, this should be the Amazon Web Services account ID.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-import-catalog-to-glue-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: ImportCatalogToGlueRequest
---
