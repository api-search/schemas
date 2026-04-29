---
description: PciDocumentInfo schema from Adyen API
layout: schema
name: PciDocumentInfo
properties_list:
- description: The date the questionnaire was created, in ISO 8601 extended format. For example, 2022-12-18T10:15:30+01:00
  name: createdAt
  type: string
- description: The unique identifier of the signed questionnaire.
  name: id
  type: string
- description: The expiration date of the questionnaire, in ISO 8601 extended format. For example, 2022-12-18T10:15:30+01:00
  name: validUntil
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-pci-document-info-schema.json
slug: legal-entity-pci-document-info
source_filename: legal-entity-pci-document-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-pci-document-info-schema.json\",\n  \"title\": \"PciDocumentInfo\",\n  \"description\": \"PciDocumentInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"createdAt\": {\n      \"description\": \"The date the questionnaire was created, in ISO 8601 extended format. For example, 2022-12-18T10:15:30+01:00\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the signed questionnaire.\",\n      \"type\": \"string\"\n    },\n    \"validUntil\": {\n      \"description\": \"The expiration date of the questionnaire, in ISO 8601 extended format. For example, 2022-12-18T10:15:30+01:00\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-pci-document-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PciDocumentInfo
---
