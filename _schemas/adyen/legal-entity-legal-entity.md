---
description: LegalEntity schema from Adyen API
layout: schema
name: LegalEntity
properties_list:
- description: 'Contains key-value pairs that specify the actions that the legal entity can do in your platform.The key is a capability required for your integration. For example, **issueCard** for Issuing.The value '
  name: capabilities
  type: object
- description: List of documents uploaded for the legal entity.
  name: documentDetails
  type: array
- description: List of documents uploaded for the legal entity.
  name: documents
  type: array
- description: List of legal entities associated with the current legal entity. For example, ultimate beneficial owners associated with an organization through ownership or control, or as signatories.
  name: entityAssociations
  type: array
- description: The unique identifier of the legal entity.
  name: id
  type: string
- description: Information about the individual. Required if `type` is **individual**.
  name: individual
  type: object
- description: Information about the organization. Required if `type` is **organization**.
  name: organization
  type: object
- description: List of verification errors related to capabilities for the legal entity.
  name: problems
  type: array
- description: Your reference for the legal entity, maximum 150 characters.
  name: reference
  type: string
- description: Information about the sole proprietorship. Required if `type` is **soleProprietorship**.
  name: soleProprietorship
  type: object
- description: List of transfer instruments that the legal entity owns.
  name: transferInstruments
  type: array
- description: Information about the trust. Required if `type` is **trust**.
  name: trust
  type: object
- description: 'The type of legal entity. Possible values: **individual**, **organization**, **soleProprietorship**, or **trust**.'
  name: type
  type: string
- description: Information about the unincorporated partnership. Required if `type` is **unincorporatedPartnership**.
  name: unincorporatedPartnership
  type: object
- description: List of verification deadlines and the capabilities that will be disallowed if verification errors are not resolved.
  name: verificationDeadlines
  type: array
- description: A key-value pair that specifies the [verification process](https://docs.adyen.com/marketplaces-and-platforms/collect-verification-details/) for a legal entity. Set to **upfront** for [upfront verifica
  name: verificationPlan
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-legal-entity-schema.json
slug: legal-entity-legal-entity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-legal-entity-schema.json\",\n  \"title\": \"LegalEntity\",\n  \"description\": \"LegalEntity schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"capabilities\": {\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/LegalEntityCapability\"\n      },\n      \"description\": \"Contains key-value pairs that specify the actions that the legal entity can do in your platform.The key is a capability required for your integration. For example, **issueCard** for Issuing.The value is an object containing the settings for the capability.\",\n      \"readOnly\": true,\n      \"type\": \"object\"\n    },\n    \"documentDetails\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"List of documents uploaded for the legal entity.\",\n      \"items\": {\n\
  \        \"$ref\": \"#/components/schemas/DocumentReference\"\n      },\n      \"type\": \"array\"\n    },\n    \"documents\": {\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"1\",\n      \"x-deprecatedMessage\": \"Use the `documentDetails` array instead.\",\n      \"description\": \"List of documents uploaded for the legal entity.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/EntityReference\"\n      },\n      \"type\": \"array\"\n    },\n    \"entityAssociations\": {\n      \"description\": \"List of legal entities associated with the current legal entity.\\nFor example, ultimate beneficial owners associated with an organization through ownership or control, or as signatories.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LegalEntityAssociation\"\n      },\n      \"type\": \"array\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the legal entity.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\
  \n    },\n    \"individual\": {\n      \"description\": \"Information about the individual. Required if `type` is **individual**.\",\n      \"$ref\": \"#/components/schemas/Individual\"\n    },\n    \"organization\": {\n      \"description\": \"Information about the organization. Required if `type` is **organization**.\",\n      \"$ref\": \"#/components/schemas/Organization\"\n    },\n    \"problems\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"List of verification errors related to capabilities for the legal entity.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CapabilityProblem\"\n      },\n      \"type\": \"array\"\n    },\n    \"reference\": {\n      \"description\": \"Your reference for the legal entity, maximum 150 characters.\",\n      \"maxLength\": 150,\n      \"type\": \"string\"\n    },\n    \"soleProprietorship\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"Information about the sole proprietorship. Required if `type`\
  \ is **soleProprietorship**.\",\n      \"$ref\": \"#/components/schemas/SoleProprietorship\"\n    },\n    \"transferInstruments\": {\n      \"description\": \"List of transfer instruments that the legal entity owns.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TransferInstrumentReference\"\n      },\n      \"readOnly\": true,\n      \"type\": \"array\"\n    },\n    \"trust\": {\n      \"description\": \"Information about the trust. Required if `type` is **trust**.\",\n      \"$ref\": \"#/components/schemas/Trust\"\n    },\n    \"type\": {\n      \"description\": \"The type of legal entity.\\n\\nPossible values: **individual**, **organization**, **soleProprietorship**, or **trust**.\",\n      \"enum\": [\n        \"individual\",\n        \"organization\",\n        \"soleProprietorship\",\n        \"trust\",\n        \"unincorporatedPartnership\"\n      ],\n      \"type\": \"string\"\n    },\n    \"unincorporatedPartnership\": {\n      \"description\": \"Information about\
  \ the unincorporated partnership. Required if `type` is **unincorporatedPartnership**.\",\n      \"$ref\": \"#/components/schemas/UnincorporatedPartnership\"\n    },\n    \"verificationDeadlines\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"List of verification deadlines and the capabilities that will be disallowed if verification errors are not resolved.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/VerificationDeadline\"\n      },\n      \"readOnly\": true,\n      \"type\": \"array\"\n    },\n    \"verificationPlan\": {\n      \"description\": \"A key-value pair that specifies the [verification process](https://docs.adyen.com/marketplaces-and-platforms/collect-verification-details/) for a legal entity. Set to **upfront** for [upfront verification](https://docs.adyen.com/marketplaces-and-platforms/collect-verification-details#upfront).\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-legal-entity-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: LegalEntity
---
