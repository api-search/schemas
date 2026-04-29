---
description: PciSigningResponse schema from Adyen API
layout: schema
name: PciSigningResponse
properties_list:
- description: The unique identifiers of the signed PCI documents.
  name: pciQuestionnaireIds
  type: array
- description: The [legal entity ID](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/legalEntities__resParam_id) of the individual who signed the PCI questionnaire.
  name: signedBy
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-pci-signing-response-schema.json
slug: legal-entity-pci-signing-response
source_filename: legal-entity-pci-signing-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-pci-signing-response-schema.json\",\n  \"title\": \"PciSigningResponse\",\n  \"description\": \"PciSigningResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pciQuestionnaireIds\": {\n      \"description\": \"The unique identifiers of the signed PCI documents.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"signedBy\": {\n      \"description\": \"The [legal entity ID](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/legalEntities__resParam_id) of the individual who signed the PCI questionnaire.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-pci-signing-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PciSigningResponse
---
