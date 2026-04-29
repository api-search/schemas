---
description: An electronic bill of lading (eBoL) or sea waybill (SWB) managed through the CargoDocs platform, representing a document of title for shipped cargo.
layout: schema
name: CargoDocs Bill of Lading
properties_list:
- description: The unique identifier for the bill of lading document.
  name: documentId
  type: string
- description: The type of bill of lading document.
  name: documentType
  type: string
- description: The unique identifier for the transaction this bill of lading belongs to.
  name: transactionId
  type: string
- description: The current status of the bill of lading (e.g., draft, issued, surrendered).
  name: status
  type: string
- description: The unique identifier for the draft version of this bill of lading.
  name: draftId
  type: string
- description: Details of the shipper named on the bill of lading.
  name: shipperDetails
  type: object
- description: Details of the consignee named on the bill of lading.
  name: consigneeDetails
  type: object
- description: Details of the cargo described on the bill of lading.
  name: cargoDetails
  type: object
- description: The timestamp when the bill of lading was issued.
  name: issuedAt
  type: string
- description: The timestamp when the bill of lading was created.
  name: createdAt
  type: string
provider_name: CargoDocs
provider_slug: cargodocs
schema_file: json-schema/cargodocs-bill-of-lading.json
slug: cargodocs-bill-of-lading
source_filename: cargodocs-bill-of-lading.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/json-schema/cargodocs-bill-of-lading.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CargoDocs Bill of Lading\",\n  \"description\": \"An electronic bill of lading (eBoL) or sea waybill (SWB) managed through the CargoDocs platform, representing a document of title for shipped cargo.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"documentId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the bill of lading document.\"\n    },\n    \"documentType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of bill of lading document.\",\n      \"enum\": [\n        \"eBoL\",\n        \"SWB\"\n      ]\n    },\n    \"transactionId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the transaction this bill of lading belongs to.\"\n    },\n    \"status\": {\n \
  \     \"type\": \"string\",\n      \"description\": \"The current status of the bill of lading (e.g., draft, issued, surrendered).\"\n    },\n    \"draftId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the draft version of this bill of lading.\"\n    },\n    \"shipperDetails\": {\n      \"type\": \"object\",\n      \"description\": \"Details of the shipper named on the bill of lading.\"\n    },\n    \"consigneeDetails\": {\n      \"type\": \"object\",\n      \"description\": \"Details of the consignee named on the bill of lading.\"\n    },\n    \"cargoDetails\": {\n      \"type\": \"object\",\n      \"description\": \"Details of the cargo described on the bill of lading.\"\n    },\n    \"issuedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the bill of lading was issued.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"The timestamp when the bill of lading was created.\"\n    }\n  },\n  \"required\": [\n    \"documentId\",\n    \"documentType\",\n    \"transactionId\",\n    \"status\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/json-schema/cargodocs-bill-of-lading.json
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
title: CargoDocs Bill of Lading
---
