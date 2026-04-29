---
description: DefenseReasonsResponse schema from Adyen API
layout: schema
name: DefenseReasonsResponse
properties_list:
- description: The defense reasons that can be used to defend the dispute.
  name: defenseReasons
  type: array
- description: The result of the dispute service.
  name: disputeServiceResult
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/disputes-defense-reasons-response-schema.json
slug: disputes-defense-reasons-response
source_filename: disputes-defense-reasons-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/disputes-defense-reasons-response-schema.json\",\n  \"title\": \"DefenseReasonsResponse\",\n  \"description\": \"DefenseReasonsResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"defenseReasons\": {\n      \"description\": \"The defense reasons that can be used to defend the dispute.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DefenseReason\"\n      },\n      \"type\": \"array\"\n    },\n    \"disputeServiceResult\": {\n      \"description\": \"The result of the dispute service.\",\n      \"$ref\": \"#/components/schemas/DisputeServiceResult\"\n    }\n  },\n  \"required\": [\n    \"disputeServiceResult\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/disputes-defense-reasons-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DefenseReasonsResponse
---
