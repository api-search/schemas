---
description: Response containing results for all created/updated fields
layout: schema
name: UpsertMetadataResponse
properties_list:
- description: Indicates if the upsert operation was successful
  name: success
  type: boolean
- description: Maps object name -> field name -> upsert result
  name: fields
  type: object
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-upsert-metadata-response-schema.json
slug: ampersand-api-upsert-metadata-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-upsert-metadata-response-schema.json\",\n  \"title\": \"UpsertMetadataResponse\",\n  \"description\": \"Response containing results for all created/updated fields\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates if the upsert operation was successful\"\n    },\n    \"fields\": {\n      \"type\": \"object\",\n      \"description\": \"Maps object name -> field name -> upsert result\",\n      \"additionalProperties\": {\n        \"type\": \"object\",\n        \"additionalProperties\": {\n          \"$ref\": \"#/components/schemas/FieldUpsertResult\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"success\",\n    \"fields\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-upsert-metadata-response-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: UpsertMetadataResponse
---
