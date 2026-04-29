---
description: LegalEntityCapability schema from Adyen API
layout: schema
name: LegalEntityCapability
properties_list:
- description: Indicates whether the capability is allowed. Adyen sets this to **true** if the verification is successful.
  name: allowed
  type: boolean
- description: 'The capability level that is allowed for the legal entity. Possible values: **notApplicable**, **low**, **medium**, **high**.'
  name: allowedLevel
  type: string
- description: The settings that are allowed for the legal entity.
  name: allowedSettings
  type: object
- description: Indicates whether the capability is requested. To check whether the legal entity is permitted to use the capability, refer to the `allowed` field.
  name: requested
  type: boolean
- description: The requested level of the capability. Some capabilities, such as those used in [card issuing](https://docs.adyen.com/issuing/add-capabilities#capability-levels), have different levels. Levels increas
  name: requestedLevel
  type: string
- description: The settings that are requested for the legal entity.
  name: requestedSettings
  type: object
- description: The capability status of transfer instruments associated with the legal entity.
  name: transferInstruments
  type: array
- description: 'The status of the verification checks for the capability. Possible values: * **pending**: Adyen is running the verification. * **invalid**: The verification failed. Check if the `errors` array contain'
  name: verificationStatus
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-legal-entity-capability-schema.json
slug: legal-entity-legal-entity-capability
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-legal-entity-capability-schema.json\",\n  \"title\": \"LegalEntityCapability\",\n  \"description\": \"LegalEntityCapability schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowed\": {\n      \"description\": \"Indicates whether the capability is allowed. Adyen sets this to **true** if the verification is successful.\",\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    },\n    \"allowedLevel\": {\n      \"description\": \"The capability level that is allowed for the legal entity.\\n\\nPossible values: **notApplicable**, **low**, **medium**, **high**.\",\n      \"enum\": [\n        \"high\",\n        \"low\",\n        \"medium\",\n        \"notApplicable\"\n      ],\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"allowedSettings\": {\n  \
  \    \"description\": \"The settings that are allowed for the legal entity.\",\n      \"readOnly\": true,\n      \"$ref\": \"#/components/schemas/CapabilitySettings\"\n    },\n    \"requested\": {\n      \"description\": \"Indicates whether the capability is requested. To check whether the legal entity is permitted to use the capability, refer to the `allowed` field.\",\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    },\n    \"requestedLevel\": {\n      \"description\": \"The requested level of the capability. Some capabilities, such as those used in [card issuing](https://docs.adyen.com/issuing/add-capabilities#capability-levels), have different levels. Levels increase the capability, but also require additional checks and increased monitoring.\\n\\nPossible values: **notApplicable**, **low**, **medium**, **high**.\",\n      \"enum\": [\n        \"high\",\n        \"low\",\n        \"medium\",\n        \"notApplicable\"\n      ],\n      \"readOnly\": true,\n      \"type\"\
  : \"string\"\n    },\n    \"requestedSettings\": {\n      \"description\": \"The settings that are requested for the legal entity.\",\n      \"readOnly\": true,\n      \"$ref\": \"#/components/schemas/CapabilitySettings\"\n    },\n    \"transferInstruments\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The capability status of transfer instruments associated with the legal entity.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SupportingEntityCapability\"\n      },\n      \"readOnly\": true,\n      \"type\": \"array\"\n    },\n    \"verificationStatus\": {\n      \"description\": \"The status of the verification checks for the capability.\\n\\nPossible values:\\n\\n* **pending**: Adyen is running the verification.\\n\\n* **invalid**: The verification failed. Check if the `errors` array contains more information.\\n\\n* **valid**: The verification has been successfully completed.\\n\\n* **rejected**: Adyen has verified the information, but found reasons\
  \ to not allow the capability.\\n\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-legal-entity-capability-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: LegalEntityCapability
---
