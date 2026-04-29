---
description: AccountHolderCapability schema from Adyen API
layout: schema
name: AccountHolderCapability
properties_list:
- description: Indicates whether the capability is allowed. Adyen sets this to **true** if the verification is successful and the account holder is permitted to use the capability.
  name: allowed
  type: boolean
- description: 'The capability level that is allowed for the account holder. Possible values: **notApplicable**, **low**, **medium**, **high**.'
  name: allowedLevel
  type: string
- description: A JSON object containing the settings that are allowed for the account holder.
  name: allowedSettings
  type: object
- description: Indicates whether the capability is enabled. If **false**, the capability is temporarily disabled for the account holder.
  name: enabled
  type: boolean
- description: Contains verification errors and the actions that you can take to resolve them.
  name: problems
  type: array
- description: Indicates whether the capability is requested. To check whether the account holder is permitted to use the capability, refer to the `allowed` field.
  name: requested
  type: boolean
- description: The requested level of the capability. Some capabilities, such as those used in [card issuing](https://docs.adyen.com/issuing/add-capabilities#capability-levels), have different levels. Levels increas
  name: requestedLevel
  type: string
- description: A JSON object containing the settings that were requested for the account holder.
  name: requestedSettings
  type: object
- description: Contains the status of the transfer instruments associated with this capability.
  name: transferInstruments
  type: array
- description: 'The status of the verification checks for the capability. Possible values: * **pending**: Adyen is running the verification. * **invalid**: The verification failed. Check if the `errors` array contain'
  name: verificationStatus
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-account-holder-capability-schema.json
slug: configuration-account-holder-capability
source_filename: configuration-account-holder-capability-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-account-holder-capability-schema.json\",\n  \"title\": \"AccountHolderCapability\",\n  \"description\": \"AccountHolderCapability schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowed\": {\n      \"description\": \"Indicates whether the capability is allowed. Adyen sets this to **true** if the verification is successful and the account holder is permitted to use the capability.\",\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    },\n    \"allowedLevel\": {\n      \"description\": \"The capability level that is allowed for the account holder.\\n\\nPossible values: **notApplicable**, **low**, **medium**, **high**.\",\n      \"enum\": [\n        \"high\",\n        \"low\",\n        \"medium\",\n        \"notApplicable\"\n      ],\n      \"readOnly\": true,\n\
  \      \"type\": \"string\"\n    },\n    \"allowedSettings\": {\n      \"description\": \"A JSON object containing the settings that are allowed for the account holder.\",\n      \"readOnly\": true,\n      \"$ref\": \"#/components/schemas/CapabilitySettings\"\n    },\n    \"enabled\": {\n      \"description\": \"Indicates whether the capability is enabled. If **false**, the capability is temporarily disabled for the account holder.\",\n      \"type\": \"boolean\"\n    },\n    \"problems\": {\n      \"description\": \"Contains verification errors and the actions that you can take to resolve them.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CapabilityProblem\"\n      },\n      \"readOnly\": true,\n      \"type\": \"array\"\n    },\n    \"requested\": {\n      \"description\": \"Indicates whether the capability is requested. To check whether the account holder is permitted to use the capability, refer to the `allowed` field.\",\n      \"type\": \"boolean\"\n    },\n \
  \   \"requestedLevel\": {\n      \"description\": \"The requested level of the capability. Some capabilities, such as those used in [card issuing](https://docs.adyen.com/issuing/add-capabilities#capability-levels), have different levels. Levels increase the capability, but also require additional checks and increased monitoring.\\n\\nPossible values: **notApplicable**, **low**, **medium**, **high**.\",\n      \"enum\": [\n        \"high\",\n        \"low\",\n        \"medium\",\n        \"notApplicable\"\n      ],\n      \"type\": \"string\"\n    },\n    \"requestedSettings\": {\n      \"description\": \"A JSON object containing the settings that were requested for the account holder.\",\n      \"readOnly\": true,\n      \"$ref\": \"#/components/schemas/CapabilitySettings\"\n    },\n    \"transferInstruments\": {\n      \"description\": \"Contains the status of the transfer instruments associated with this capability. \",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AccountSupportingEntityCapability\"\
  \n      },\n      \"readOnly\": true,\n      \"type\": \"array\"\n    },\n    \"verificationStatus\": {\n      \"description\": \"The status of the verification checks for the capability.\\n\\nPossible values:\\n\\n* **pending**: Adyen is running the verification.\\n\\n* **invalid**: The verification failed. Check if the `errors` array contains more information.\\n\\n* **valid**: The verification has been successfully completed.\\n\\n* **rejected**: Adyen has verified the information, but found reasons to not allow the capability.\\n\",\n      \"enum\": [\n        \"invalid\",\n        \"pending\",\n        \"rejected\",\n        \"valid\"\n      ],\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-account-holder-capability-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AccountHolderCapability
---
