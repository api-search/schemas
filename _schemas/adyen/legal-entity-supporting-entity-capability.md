---
description: SupportingEntityCapability schema from Adyen API
layout: schema
name: SupportingEntityCapability
properties_list:
- description: Indicates whether the capability is allowed for the supporting entity. If a capability is allowed for a supporting entity but not for the parent legal entity, this means the legal entity has other sup
  name: allowed
  type: boolean
- description: Supporting entity reference
  name: id
  type: string
- description: Indicates whether the supporting entity capability is requested.
  name: requested
  type: boolean
- description: 'The status of the verification checks for the capability of the supporting entity. Possible values: * **pending**: Adyen is running the verification. * **invalid**: The verification failed. Check if t'
  name: verificationStatus
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-supporting-entity-capability-schema.json
slug: legal-entity-supporting-entity-capability
source_filename: legal-entity-supporting-entity-capability-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-supporting-entity-capability-schema.json\",\n  \"title\": \"SupportingEntityCapability\",\n  \"description\": \"SupportingEntityCapability schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowed\": {\n      \"description\": \"Indicates whether the capability is allowed for the supporting entity.\\n\\nIf a capability is allowed for a supporting entity but not for the parent legal entity, this means the legal entity has other supporting entities that failed verification.\\n\\n**You can use the allowed supporting entity** regardless of the verification status of other supporting entities.\",\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    },\n    \"id\": {\n      \"description\": \"Supporting entity reference \",\n      \"readOnly\": true,\n      \"type\": \"\
  string\"\n    },\n    \"requested\": {\n      \"description\": \"Indicates whether the supporting entity capability is requested. \",\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    },\n    \"verificationStatus\": {\n      \"description\": \"The status of the verification checks for the capability of the supporting entity.\\n\\nPossible values:\\n\\n* **pending**: Adyen is running the verification.\\n\\n* **invalid**: The verification failed. Check if the `errors` array contains more information.\\n\\n* **valid**: The verification has been successfully completed.\\n\\n* **rejected**: Adyen has verified the information, but found reasons to not allow the capability.\\n\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-supporting-entity-capability-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SupportingEntityCapability
---
