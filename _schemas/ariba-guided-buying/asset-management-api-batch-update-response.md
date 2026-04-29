---
description: Response for batch asset line item update.
layout: schema
name: BatchUpdateResponse
properties_list:
- description: Total number of records processed.
  name: processed
  type: integer
- description: Number of records successfully updated.
  name: succeeded
  type: integer
- description: Number of records that failed to update.
  name: failed
  type: integer
provider_name: Ariba Guided Buying
provider_slug: ariba-guided-buying
schema_file: json-schema/asset-management-api-batch-update-response-schema.json
slug: asset-management-api-batch-update-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/json-schema/asset-management-api-batch-update-response-schema.json\",\n  \"title\": \"BatchUpdateResponse\",\n  \"description\": \"Response for batch asset line item update.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"processed\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of records processed.\",\n      \"example\": 1\n    },\n    \"succeeded\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of records successfully updated.\",\n      \"example\": 1\n    },\n    \"failed\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of records that failed to update.\",\n      \"example\": 0\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/json-schema/asset-management-api-batch-update-response-schema.json
tags:
- B2B
- Catalog
- ERP
- Procurement
- Requisitions
- SAP
- Supply Chain
title: BatchUpdateResponse
---
