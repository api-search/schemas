---
description: AccountCapabilityData schema from Adyen API
layout: schema
name: AccountCapabilityData
properties_list:
- description: Indicates whether the capability is allowed. Adyen sets this to **true** if the verification is successful.
  name: allowed
  type: boolean
- description: 'The allowed level of the capability. Some capabilities have different levels which correspond to thresholds. Higher levels may require additional checks and increased monitoring.Possible values: **not'
  name: allowedLevel
  type: string
- description: The name of the capability. For example, **sendToTransferInstrument**.
  name: capability
  type: string
- description: List of entities that has problems with verification. The information includes the details of the errors and the actions that you can take to resolve them.
  name: problems
  type: array
- description: Indicates whether you requested the capability.
  name: requested
  type: boolean
- description: The level that you requested for the capability. Some capabilities have different levels which correspond to thresholds. Higher levels may require additional checks and increased monitoring.Possible v
  name: requestedLevel
  type: string
- description: The verification deadline for the capability that will be disallowed if verification errors are not resolved.
  name: verificationDeadline
  type: string
- description: 'The status of the verification checks for the capability. Possible values: * **pending**: Adyen is running the verification. * **invalid**: The verification failed. Check if the `errors` array contain'
  name: verificationStatus
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-webhooks-account-capability-data-schema.json
slug: management-webhooks-account-capability-data
source_filename: management-webhooks-account-capability-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-webhooks-account-capability-data-schema.json\",\n  \"title\": \"AccountCapabilityData\",\n  \"description\": \"AccountCapabilityData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowed\": {\n      \"description\": \"Indicates whether the capability is allowed. Adyen sets this to **true** if the verification is successful.\",\n      \"type\": \"boolean\"\n    },\n    \"allowedLevel\": {\n      \"description\": \"The allowed level of the capability. Some capabilities have different levels which correspond to thresholds. Higher levels may require additional checks and increased monitoring.Possible values: **notApplicable**, **low**, **medium**, **high**.\",\n      \"type\": \"string\"\n    },\n    \"capability\": {\n      \"description\": \"The name of the capability. For\
  \ example, **sendToTransferInstrument**.\",\n      \"type\": \"string\"\n    },\n    \"problems\": {\n      \"description\": \"List of entities that has problems with verification. The information includes the details of the errors and the actions that you can take to resolve them.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CapabilityProblem\"\n      },\n      \"type\": \"array\"\n    },\n    \"requested\": {\n      \"description\": \"Indicates whether you requested the capability.\",\n      \"type\": \"boolean\"\n    },\n    \"requestedLevel\": {\n      \"description\": \"The level that you requested for the capability. Some capabilities have different levels which correspond to thresholds. Higher levels may require additional checks and increased monitoring.Possible values: **notApplicable**, **low**, **medium**, **high**.\",\n      \"type\": \"string\"\n    },\n    \"verificationDeadline\": {\n      \"description\": \"The verification deadline for the capability\
  \ that will be disallowed if verification errors are not resolved.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"verificationStatus\": {\n      \"description\": \"The status of the verification checks for the capability.\\n\\nPossible values:\\n\\n* **pending**: Adyen is running the verification.\\n\\n* **invalid**: The verification failed. Check if the `errors` array contains more information.\\n\\n* **valid**: The verification was successful.\\n\\n* **rejected**: Adyen checked the information and found reasons to not allow the capability.\\n\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"requestedLevel\",\n    \"requested\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-webhooks-account-capability-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AccountCapabilityData
---
