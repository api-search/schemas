---
description: CapabilityProblem schema from Adyen API
layout: schema
name: CapabilityProblem
properties_list:
- description: Contains the type of the entity and the corresponding ID.
  name: entity
  type: object
- description: Contains information about the verification error.
  name: verificationErrors
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-capability-problem-schema.json
slug: notification-webhooks-capability-problem
source_filename: notification-webhooks-capability-problem-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-capability-problem-schema.json\",\n  \"title\": \"CapabilityProblem\",\n  \"description\": \"CapabilityProblem schema from Adyen API\",\n  \"properties\": {\n    \"entity\": {\n      \"description\": \"Contains the type of the entity and the corresponding ID.\",\n      \"$ref\": \"#/components/schemas/CapabilityProblemEntity\"\n    },\n    \"verificationErrors\": {\n      \"description\": \"Contains information about the verification error.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/VerificationError\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-capability-problem-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CapabilityProblem
---
