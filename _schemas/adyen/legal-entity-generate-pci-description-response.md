---
description: GeneratePciDescriptionResponse schema from Adyen API
layout: schema
name: GeneratePciDescriptionResponse
properties_list:
- description: The generated questionnaires in a base64 encoded format.
  name: content
  type: string
- description: The two-letter [ISO-639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) language code for the questionnaire. For example, **en**.
  name: language
  type: string
- description: The array of Adyen-generated unique identifiers for the questionnaires.
  name: pciTemplateReferences
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-generate-pci-description-response-schema.json
slug: legal-entity-generate-pci-description-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-generate-pci-description-response-schema.json\",\n  \"title\": \"GeneratePciDescriptionResponse\",\n  \"description\": \"GeneratePciDescriptionResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {\n      \"description\": \"The generated questionnaires in a base64 encoded format.\",\n      \"format\": \"byte\",\n      \"type\": \"string\"\n    },\n    \"language\": {\n      \"description\": \"The two-letter [ISO-639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) language code for the questionnaire. For example, **en**.\",\n      \"type\": \"string\"\n    },\n    \"pciTemplateReferences\": {\n      \"description\": \"The array of Adyen-generated unique identifiers for the questionnaires.\",\n      \"items\": {\n        \"type\": \"string\"\n   \
  \   },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-generate-pci-description-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: GeneratePciDescriptionResponse
---
