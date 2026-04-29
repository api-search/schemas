---
description: LegalEntityAssociation schema from Adyen API
layout: schema
name: LegalEntityAssociation
properties_list:
- description: The unique identifier of another legal entity with which the `legalEntityId` is associated. When the `legalEntityId` is associated to legal entities other than the current one, the response returns al
  name: associatorId
  type: string
- description: The legal entity type of associated legal entity. For example, **organization**, **soleProprietorship** or **individual**.
  name: entityType
  type: string
- description: The individual's job title if the `type` is **uboThroughControl** or **signatory**.
  name: jobTitle
  type: string
- description: The unique identifier of the associated [legal entity](https://docs.adyen.com/api-explorer/legalentity/latest/post/legalEntities#responses-200-id).
  name: legalEntityId
  type: string
- description: The name of the associated [legal entity](https://docs.adyen.com/api-explorer/legalentity/latest/post/legalEntities#responses-200-id). - For **individual**, `name.firstName` and `name.lastName`. - For
  name: name
  type: string
- description: Defines the Kyc Exemption Reason for a Settlor associated with a trust. For example, **professionalServiceProvider**, **deceased**, or **contributionBelowThreshold**.
  name: settlorExemptionReason
  type: array
- description: 'Defines the relationship of the legal entity to the current legal entity. Possible values for organizations: **uboThroughOwnership**, **uboThroughControl**, **director**, **signatory**, or **ultimateP'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-legal-entity-association-schema.json
slug: legal-entity-legal-entity-association
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-legal-entity-association-schema.json\",\n  \"title\": \"LegalEntityAssociation\",\n  \"description\": \"LegalEntityAssociation schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"associatorId\": {\n      \"description\": \"The unique identifier of another legal entity with which the `legalEntityId` is associated. When the `legalEntityId` is associated to legal entities other than the current one, the response returns all the associations.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"entityType\": {\n      \"description\": \"The legal entity type of associated legal entity.\\n\\nFor example, **organization**, **soleProprietorship** or **individual**.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"jobTitle\": {\n      \"description\"\
  : \"The individual's job title if the `type` is **uboThroughControl** or **signatory**.\",\n      \"type\": \"string\"\n    },\n    \"legalEntityId\": {\n      \"description\": \"The unique identifier of the associated [legal entity](https://docs.adyen.com/api-explorer/legalentity/latest/post/legalEntities#responses-200-id).\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The name of the associated [legal entity](https://docs.adyen.com/api-explorer/legalentity/latest/post/legalEntities#responses-200-id).\\n\\n- For **individual**, `name.firstName` and `name.lastName`.\\n- For **organization**, `legalName`.\\n- For **soleProprietorship**, `name`.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"settlorExemptionReason\": {\n      \"description\": \"Defines the Kyc Exemption Reason for a Settlor associated with a trust.\\n\\nFor example, **professionalServiceProvider**, **deceased**, or **contributionBelowThreshold**.\",\n      \"\
  items\": {\n        \"type\": \"string\"\n      },\n      \"readOnly\": true,\n      \"type\": \"array\"\n    },\n    \"type\": {\n      \"description\": \"Defines the relationship of the legal entity to the current legal entity.\\n\\nPossible values for organizations: **uboThroughOwnership**, **uboThroughControl**, **director**, **signatory**, or **ultimateParentCompany**.\\n\\nPossible values for sole proprietorships: **soleProprietorship**.\\n\\nPossible value for trusts: **trust**\\n\\nPossible values for trust members: **definedBeneficiary**, **protector**, **secondaryTrustee**, **settlor**, **uboThroughControl**, or **uboThroughOwnership**.\",\n      \"enum\": [\n        \"definedBeneficiary\",\n        \"director\",\n        \"pciSignatory\",\n        \"protector\",\n        \"secondaryTrustee\",\n        \"settlor\",\n        \"signatory\",\n        \"soleProprietorship\",\n        \"trust\",\n        \"trustOwnership\",\n        \"uboThroughControl\",\n        \"uboThroughOwnership\"\
  ,\n        \"ultimateParentCompany\",\n        \"undefinedBeneficiary\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"legalEntityId\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-legal-entity-association-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: LegalEntityAssociation
---
