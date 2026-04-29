---
description: A purchase requisition with asset line items.
layout: schema
name: Requisition
properties_list:
- description: Requisition identifier.
  name: id
  type: string
- description: Requisition title or description.
  name: title
  type: string
- description: Current status of the requisition.
  name: status
  type: string
- description: Date and time the requisition was created.
  name: createdDate
  type: string
- description: Date and time the requisition was last updated.
  name: updatedDate
  type: string
- description: Line items in the requisition.
  name: lineItems
  type: array
provider_name: Ariba Guided Buying
provider_slug: ariba-guided-buying
schema_file: json-schema/asset-management-api-requisition-schema.json
slug: asset-management-api-requisition
source_filename: asset-management-api-requisition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/json-schema/asset-management-api-requisition-schema.json\",\n  \"title\": \"Requisition\",\n  \"description\": \"A purchase requisition with asset line items.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Requisition identifier.\",\n      \"example\": \"REQ-500123\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Requisition title or description.\",\n      \"example\": \"Office Equipment Purchase\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the requisition.\",\n      \"example\": \"InProgress\",\n      \"enum\": [\n        \"InProgress\",\n        \"Completed\",\n        \"Approved\",\n        \"Pending\"\n      ]\n    },\n    \"createdDate\": {\n  \
  \    \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the requisition was created.\",\n      \"example\": \"2026-01-15T09:00:00Z\"\n    },\n    \"updatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the requisition was last updated.\",\n      \"example\": \"2026-01-16T10:00:00Z\"\n    },\n    \"lineItems\": {\n      \"type\": \"array\",\n      \"description\": \"Line items in the requisition.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AssetLineItem\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/json-schema/asset-management-api-requisition-schema.json
tags:
- B2B
- Catalog
- ERP
- Procurement
- Requisitions
- SAP
- Supply Chain
title: Requisition
---
