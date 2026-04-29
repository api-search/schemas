---
description: AccountSupportingEntityCapability schema from Adyen API
layout: schema
name: AccountSupportingEntityCapability
properties_list:
- description: Indicates whether the supporting entity capability is allowed. Adyen sets this to **true** if the verification is successful and the account holder is permitted to use the capability.
  name: allowed
  type: boolean
- description: 'The capability level that is allowed for the account holder. Possible values: **notApplicable**, **low**, **medium**, **high**.'
  name: allowedLevel
  type: string
- description: Indicates whether the capability is enabled. If **false**, the capability is temporarily disabled for the account holder.
  name: enabled
  type: boolean
- description: The ID of the supporting entity.
  name: id
  type: string
- description: Indicates whether the capability is requested. To check whether the account holder is permitted to use the capability, refer to the `allowed` field.
  name: requested
  type: boolean
- description: The requested level of the capability. Some capabilities, such as those used in [card issuing](https://docs.adyen.com/issuing/add-capabilities#capability-levels), have different levels. Levels increas
  name: requestedLevel
  type: string
- description: 'The status of the verification checks for the supporting entity capability. Possible values: * **pending**: Adyen is running the verification. * **invalid**: The verification failed. Check if the `err'
  name: verificationStatus
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-webhooks-account-supporting-entity-capability-schema.json
slug: configuration-webhooks-account-supporting-entity-capability
source_filename: configuration-webhooks-account-supporting-entity-capability-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-account-supporting-entity-capability-schema.json\",\n  \"title\": \"AccountSupportingEntityCapability\",\n  \"description\": \"AccountSupportingEntityCapability schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowed\": {\n      \"description\": \"Indicates whether the supporting entity capability is allowed. Adyen sets this to **true** if the verification is successful and the account holder is permitted to use the capability.\",\n      \"type\": \"boolean\"\n    },\n    \"allowedLevel\": {\n      \"description\": \"The capability level that is allowed for the account holder.\\n\\nPossible values: **notApplicable**, **low**, **medium**, **high**.\",\n      \"enum\": [\n        \"high\",\n        \"low\",\n        \"medium\",\n        \"notApplicable\"\n     \
  \ ],\n      \"type\": \"string\"\n    },\n    \"enabled\": {\n      \"description\": \"Indicates whether the capability is enabled. If **false**, the capability is temporarily disabled for the account holder.\",\n      \"type\": \"boolean\"\n    },\n    \"id\": {\n      \"description\": \"The ID of the supporting entity.\",\n      \"type\": \"string\"\n    },\n    \"requested\": {\n      \"description\": \"Indicates whether the capability is requested. To check whether the account holder is permitted to use the capability, refer to the `allowed` field.\",\n      \"type\": \"boolean\"\n    },\n    \"requestedLevel\": {\n      \"description\": \"The requested level of the capability. Some capabilities, such as those used in [card issuing](https://docs.adyen.com/issuing/add-capabilities#capability-levels), have different levels. Levels increase the capability, but also require additional checks and increased monitoring.\\n\\nPossible values: **notApplicable**, **low**, **medium**, **high**.\"\
  ,\n      \"enum\": [\n        \"high\",\n        \"low\",\n        \"medium\",\n        \"notApplicable\"\n      ],\n      \"type\": \"string\"\n    },\n    \"verificationStatus\": {\n      \"description\": \"The status of the verification checks for the supporting entity capability.\\n\\nPossible values:\\n\\n* **pending**: Adyen is running the verification.\\n\\n* **invalid**: The verification failed. Check if the `errors` array contains more information.\\n\\n* **valid**: The verification has been successfully completed.\\n\\n* **rejected**: Adyen has verified the information, but found reasons to not allow the capability.\\n\",\n      \"enum\": [\n        \"invalid\",\n        \"pending\",\n        \"rejected\",\n        \"valid\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-account-supporting-entity-capability-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AccountSupportingEntityCapability
---
