---
description: LegalArrangementDetail schema from Adyen API
layout: schema
name: LegalArrangementDetail
properties_list:
- description: The address of the legal arrangement.
  name: address
  type: object
- description: Adyen-generated unique alphanumeric identifier (UUID) for the entry, returned in the response when you create a legal arrangement. Use only when updating an account holder. If you include this field w
  name: legalArrangementCode
  type: string
- description: An array containing information about other entities that are part of the legal arrangement.
  name: legalArrangementEntities
  type: array
- description: Your reference for the legal arrangement. Must be between 3 to 128 characters.
  name: legalArrangementReference
  type: string
- description: 'The form of legal arrangement. Required if `type` is **Trust** or **Partnership**. The possible values depend on the `type`. - For `type` **Trust**: **CashManagementTrust**, **CorporateUnitTrust**, **'
  name: legalForm
  type: string
- description: 'The legal name of the legal arrangement. Minimum length: 3 characters.'
  name: name
  type: string
- description: The registration number of the legal arrangement.
  name: registrationNumber
  type: string
- description: The tax identification number of the legal arrangement.
  name: taxNumber
  type: string
- description: 'The [type of legal arrangement](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/legal-arrangements#types-of-legal-arrangements). Possible values: - **Association** - **P'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-legal-arrangement-detail-schema.json
slug: accounts-legal-arrangement-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-legal-arrangement-detail-schema.json\",\n  \"title\": \"LegalArrangementDetail\",\n  \"description\": \"LegalArrangementDetail schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"description\": \"The address of the legal arrangement.\",\n      \"$ref\": \"#/components/schemas/ViasAddress\"\n    },\n    \"legalArrangementCode\": {\n      \"description\": \"Adyen-generated unique alphanumeric identifier (UUID) for the entry, returned in the response when you create a legal arrangement.\\nUse only when updating an account holder. If you include this field when creating an account holder, the request will fail.\",\n      \"type\": \"string\"\n    },\n    \"legalArrangementEntities\": {\n      \"description\": \"An array containing information about other entities\
  \ that are part of the legal arrangement.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LegalArrangementEntityDetail\"\n      },\n      \"type\": \"array\"\n    },\n    \"legalArrangementReference\": {\n      \"description\": \"Your reference for the legal arrangement. Must be between 3 to 128 characters.\",\n      \"type\": \"string\"\n    },\n    \"legalForm\": {\n      \"description\": \"The form of legal arrangement. Required if `type` is **Trust** or **Partnership**.\\n\\nThe possible values depend on the `type`.\\n\\n- For `type` **Trust**:  **CashManagementTrust**, **CorporateUnitTrust**, **DeceasedEstate**, **DiscretionaryInvestmentTrust**, **DiscretionaryServicesManagementTrust**, **DiscretionaryTradingTrust**, **FirstHomeSaverAccountsTrust**, **FixedTrust**, **FixedUnitTrust**, **HybridTrust**, **ListedPublicUnitTrust**, **OtherTrust**, **PooledSuperannuationTrust**, **PublicTradingTrust**, or **UnlistedPublicUnitTrust**.\\n\\n- For `type` **Partnership**:\
  \ **LimitedPartnership**, **FamilyPartnership**, or **OtherPartnership**\",\n      \"enum\": [\n        \"CashManagementTrust\",\n        \"CorporateUnitTrust\",\n        \"DeceasedEstate\",\n        \"DiscretionaryInvestmentTrust\",\n        \"DiscretionaryServicesManagementTrust\",\n        \"DiscretionaryTradingTrust\",\n        \"FirstHomeSaverAccountsTrust\",\n        \"FixedTrust\",\n        \"FixedUnitTrust\",\n        \"HybridTrust\",\n        \"ListedPublicUnitTrust\",\n        \"OtherTrust\",\n        \"PooledSuperannuationTrust\",\n        \"PublicTradingTrust\",\n        \"UnlistedPublicUnitTrust\",\n        \"LimitedPartnership\",\n        \"FamilyPartnership\",\n        \"OtherPartnership\"\n      ],\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The legal name of the legal arrangement. Minimum length: 3 characters.\",\n      \"type\": \"string\"\n    },\n    \"registrationNumber\": {\n      \"description\": \"The registration number of the\
  \ legal arrangement.\",\n      \"type\": \"string\"\n    },\n    \"taxNumber\": {\n      \"description\": \"The tax identification number of the legal arrangement.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The [type of legal arrangement](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/legal-arrangements#types-of-legal-arrangements).\\n\\nPossible values:\\n\\n- **Association** \\n\\n- **Partnership** \\n\\n- **SoleProprietorship** \\n\\n- **Trust** \\n\\n\",\n      \"enum\": [\n        \"Association\",\n        \"Partnership\",\n        \"SoleProprietorship\",\n        \"Trust\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"name\",\n    \"address\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-legal-arrangement-detail-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: LegalArrangementDetail
---
