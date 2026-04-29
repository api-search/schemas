---
description: GeneratePciDescriptionRequest schema from Adyen API
layout: schema
name: GeneratePciDescriptionRequest
properties_list:
- description: An array of additional sales channels to generate PCI questionnaires. Include the relevant sales channels if you need your user to sign PCI questionnaires. Not required if you [create stores](https://
  name: additionalSalesChannels
  type: array
- description: Sets the language of the PCI questionnaire. Its value is a two-character [ISO 639-1](https://en.wikipedia.org/wiki/ISO_639-1) language code, for example, **en**.
  name: language
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-generate-pci-description-request-schema.json
slug: legal-entity-generate-pci-description-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-generate-pci-description-request-schema.json\",\n  \"title\": \"GeneratePciDescriptionRequest\",\n  \"description\": \"GeneratePciDescriptionRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"additionalSalesChannels\": {\n      \"description\": \"An array of additional sales channels to generate PCI questionnaires. Include the relevant sales channels if you need your user to sign PCI questionnaires. Not required if you [create stores](https://docs.adyen.com/marketplaces-and-platforms/additional-for-platform-setup/create-stores/) and [add payment methods](https://docs.adyen.com/marketplaces-and-platforms/payment-methods/) before you generate the questionnaires.\\n\\nPossible values:\\n*  **eCommerce**\\n*  **pos**\\n*  **ecomMoto**\\n*  **posMoto**\\n\\n\",\n      \"\
  items\": {\n        \"enum\": [\n          \"eCommerce\",\n          \"ecomMoto\",\n          \"pos\",\n          \"posMoto\"\n        ],\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"language\": {\n      \"description\": \"Sets the language of the PCI questionnaire. Its value is a two-character [ISO 639-1](https://en.wikipedia.org/wiki/ISO_639-1) language code, for example, **en**.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-generate-pci-description-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: GeneratePciDescriptionRequest
---
