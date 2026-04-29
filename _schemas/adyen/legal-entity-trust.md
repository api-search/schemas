---
description: Trust schema from Adyen API
layout: schema
name: Trust
properties_list:
- description: The two-character [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) country code of the governing country.
  name: countryOfGoverningLaw
  type: string
- description: The date when the legal arrangement was incorporated in YYYY-MM-DD format.
  name: dateOfIncorporation
  type: string
- description: Short description about the trust.
  name: description
  type: string
- description: The registered name, if different from the `name`.
  name: doingBusinessAs
  type: string
- description: The legal name.
  name: name
  type: string
- description: The business address. Required if the principal place of business is different from the `registeredAddress`.
  name: principalPlaceOfBusiness
  type: object
- description: The address registered at the registrar, such as the Chamber of Commerce.
  name: registeredAddress
  type: object
- description: The registration number.
  name: registrationNumber
  type: string
- description: The tax information of the entity.
  name: taxInformation
  type: array
- description: 'Type of trust. Possible values for Australian trusts: **cashManagementTrust**, **corporateUnitTrust**, **deceasedEstate**, **discretionaryInvestmentTrust**, **discretionaryServicesManagementTrust**, *'
  name: type
  type: string
- description: The undefined beneficiary information of the entity.
  name: undefinedBeneficiaryInfo
  type: array
- description: 'The reason for not providing a VAT number. Possible values: **industryExemption**, **belowTaxThreshold**.'
  name: vatAbsenceReason
  type: string
- description: The VAT number.
  name: vatNumber
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-trust-schema.json
slug: legal-entity-trust
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-trust-schema.json\",\n  \"title\": \"Trust\",\n  \"description\": \"Trust schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"countryOfGoverningLaw\": {\n      \"description\": \"The two-character [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) country code of the governing country.\",\n      \"type\": \"string\"\n    },\n    \"dateOfIncorporation\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The date when the legal arrangement was incorporated in YYYY-MM-DD format.\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"Short description about the trust.\",\n      \"type\": \"string\"\n    },\n    \"doingBusinessAs\": {\n      \"description\": \"The registered name,\
  \ if different from the `name`.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The legal name.\",\n      \"type\": \"string\"\n    },\n    \"principalPlaceOfBusiness\": {\n      \"description\": \"The business address. Required if the principal place of business is different from the `registeredAddress`.\",\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"registeredAddress\": {\n      \"description\": \"The address registered at the registrar, such as the Chamber of Commerce.\",\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"registrationNumber\": {\n      \"description\": \"The registration number.\",\n      \"type\": \"string\"\n    },\n    \"taxInformation\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The tax information of the entity.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TaxInformation\"\n      },\n      \"type\": \"array\"\n    },\n    \"type\": {\n      \"description\"\
  : \"Type of trust.\\n\\nPossible values for Australian trusts: **cashManagementTrust**, **corporateUnitTrust**, **deceasedEstate**, **discretionaryInvestmentTrust**, **discretionaryServicesManagementTrust**, **discretionaryTradingTrust**, **firstHomeSaverAccountsTrust**, **fixedTrust**, **fixedUnitTrust**, **hybridTrust**, **listedPublicUnitTrust**, **otherTrust**, **pooledSuperannuationTrust**, **publicTradingTrust**, **unlistedPublicUnitTrust**.\",\n      \"enum\": [\n        \"cashManagementTrust\",\n        \"corporateUnitTrust\",\n        \"deceasedEstate\",\n        \"discretionaryInvestmentTrust\",\n        \"discretionaryServicesManagementTrust\",\n        \"discretionaryTradingTrust\",\n        \"firstHomeSaverAccountsTrust\",\n        \"fixedTrust\",\n        \"fixedUnitTrust\",\n        \"hybridTrust\",\n        \"listedPublicUnitTrust\",\n        \"otherTrust\",\n        \"pooledSuperannuationTrust\",\n        \"publicTradingTrust\",\n        \"unlistedPublicUnitTrust\"\n \
  \     ],\n      \"type\": \"string\"\n    },\n    \"undefinedBeneficiaryInfo\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The undefined beneficiary information of the entity.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/UndefinedBeneficiary\"\n      },\n      \"type\": \"array\"\n    },\n    \"vatAbsenceReason\": {\n      \"description\": \"The reason for not providing a VAT number.\\n\\nPossible values: **industryExemption**, **belowTaxThreshold**.\",\n      \"enum\": [\n        \"industryExemption\",\n        \"belowTaxThreshold\"\n      ],\n      \"type\": \"string\"\n    },\n    \"vatNumber\": {\n      \"description\": \"The VAT number.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"countryOfGoverningLaw\",\n    \"registeredAddress\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-trust-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Trust
---
