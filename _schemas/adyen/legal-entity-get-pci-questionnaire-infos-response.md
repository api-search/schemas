---
description: GetPciQuestionnaireInfosResponse schema from Adyen API
layout: schema
name: GetPciQuestionnaireInfosResponse
properties_list:
- description: Information about the signed PCI questionnaires.
  name: data
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-get-pci-questionnaire-infos-response-schema.json
slug: legal-entity-get-pci-questionnaire-infos-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-get-pci-questionnaire-infos-response-schema.json\",\n  \"title\": \"GetPciQuestionnaireInfosResponse\",\n  \"description\": \"GetPciQuestionnaireInfosResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"description\": \"Information about the signed PCI questionnaires.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PciDocumentInfo\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-get-pci-questionnaire-infos-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: GetPciQuestionnaireInfosResponse
---
