---
description: A trade or shipping document managed within the CargoDocs platform, such as a bill of lading, certificate of origin, or invoice.
layout: schema
name: CargoDocs Document
properties_list:
- description: The unique identifier for the document.
  name: documentId
  type: string
- description: The type of document (e.g., eBoL, SWB, certificate, invoice).
  name: documentType
  type: string
- description: The current status of the document.
  name: status
  type: string
- description: The timestamp when the document was created.
  name: createdAt
  type: string
provider_name: CargoDocs
provider_slug: cargodocs
schema_file: json-schema/cargodocs-document.json
slug: cargodocs-document
source_json: "{\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/json-schema/cargodocs-document.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CargoDocs Document\",\n  \"description\": \"A trade or shipping document managed within the CargoDocs platform, such as a bill of lading, certificate of origin, or invoice.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"documentId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the document.\"\n    },\n    \"documentType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of document (e.g., eBoL, SWB, certificate, invoice).\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the document.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the document was created.\"\
  \n    }\n  },\n  \"required\": [\n    \"documentId\",\n    \"documentType\",\n    \"status\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/json-schema/cargodocs-document.json
tags:
- Bills of Lading
- Documentation
- eBoL
- EssDocs
- MLETR
- Shipping
- Supply Chain
- Trade
- Trade Finance
- Warehouse Warrants
title: CargoDocs Document
---
