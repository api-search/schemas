---
description: PciSigningRequest schema from Adyen API
layout: schema
name: PciSigningRequest
properties_list:
- description: The array of Adyen-generated unique identifiers for the questionnaires.
  name: pciTemplateReferences
  type: array
- description: The [legal entity ID](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/legalEntities__resParam_id) of the individual who signs the PCI questionnaire.
  name: signedBy
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-pci-signing-request-schema.json
slug: legal-entity-pci-signing-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-pci-signing-request-schema.json\",\n  \"title\": \"PciSigningRequest\",\n  \"description\": \"PciSigningRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pciTemplateReferences\": {\n      \"description\": \"The array of Adyen-generated unique identifiers for the questionnaires.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"signedBy\": {\n      \"description\": \"The [legal entity ID](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/legalEntities__resParam_id) of the individual who signs the PCI questionnaire.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"signedBy\",\n    \"pciTemplateReferences\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-pci-signing-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PciSigningRequest
---
