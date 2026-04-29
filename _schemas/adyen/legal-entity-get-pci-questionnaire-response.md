---
description: GetPciQuestionnaireResponse schema from Adyen API
layout: schema
name: GetPciQuestionnaireResponse
properties_list:
- description: The generated questionnaire in a base64 encoded format.
  name: content
  type: string
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
schema_file: json-schema/legal-entity-get-pci-questionnaire-response-schema.json
slug: legal-entity-get-pci-questionnaire-response
source_filename: legal-entity-get-pci-questionnaire-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-get-pci-questionnaire-response-schema.json\",\n  \"title\": \"GetPciQuestionnaireResponse\",\n  \"description\": \"GetPciQuestionnaireResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {\n      \"description\": \"The generated questionnaire in a base64 encoded format.\",\n      \"format\": \"byte\",\n      \"type\": \"string\"\n    },\n    \"createdAt\": {\n      \"description\": \"The date the questionnaire was created, in ISO 8601 extended format. For example, 2022-12-18T10:15:30+01:00\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the signed questionnaire.\",\n      \"type\": \"string\"\n    },\n    \"validUntil\": {\n      \"description\": \"The expiration date\
  \ of the questionnaire, in ISO 8601 extended format. For example, 2022-12-18T10:15:30+01:00\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-get-pci-questionnaire-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: GetPciQuestionnaireResponse
---
