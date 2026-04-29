---
description: Organization schema from Adyen API
layout: schema
name: Organization
properties_list:
- description: The date when the organization was incorporated in YYYY-MM-DD format.
  name: dateOfIncorporation
  type: string
- description: Your description for the organization.
  name: description
  type: string
- description: The organization's trading name, if different from the registered legal name.
  name: doingBusinessAs
  type: string
- description: The email address of the legal entity.
  name: email
  type: string
- description: The organization's legal name.
  name: legalName
  type: string
- description: The phone number of the legal entity.
  name: phone
  type: object
- description: The address where the organization operates from. Provide this if the principal place of business is different from the `registeredAddress`.
  name: principalPlaceOfBusiness
  type: object
- description: The address of the organization registered at their registrar (such as the Chamber of Commerce).
  name: registeredAddress
  type: object
- description: The organization's registration number.
  name: registrationNumber
  type: string
- description: Information about the organization's publicly traded stock. Provide this object only if `type` is **listedPublicCompany**.
  name: stockData
  type: object
- description: The tax information of the organization.
  name: taxInformation
  type: array
- description: The tax reporting classification (FATCA/CRS self-certification) of the organization.
  name: taxReportingClassification
  type: object
- description: 'Type of organization. Possible values: **associationIncorporated**, **governmentalOrganization**, **listedPublicCompany**, **nonProfit**, **partnershipIncorporated**, **privateCompany**.'
  name: type
  type: string
- description: 'The reason the organization has not provided a VAT number. Possible values: **industryExemption**, **belowTaxThreshold**.'
  name: vatAbsenceReason
  type: string
- description: The organization's VAT number.
  name: vatNumber
  type: string
- description: The website and app URL of the legal entity.
  name: webData
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-organization-schema.json
slug: legal-entity-organization
source_filename: legal-entity-organization-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-organization-schema.json\",\n  \"title\": \"Organization\",\n  \"description\": \"Organization schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dateOfIncorporation\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The date when the organization was incorporated in YYYY-MM-DD format.\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"description\": \"Your description for the organization.\",\n      \"type\": \"string\"\n    },\n    \"doingBusinessAs\": {\n      \"description\": \"The organization's trading name, if different from the registered legal name.\",\n      \"type\": \"string\"\n    },\n    \"email\": {\n      \"description\": \"The email address of the legal entity.\",\n      \"type\": \"string\"\n    },\n    \"legalName\":\
  \ {\n      \"description\": \"The organization's legal name.\",\n      \"type\": \"string\"\n    },\n    \"phone\": {\n      \"description\": \"The phone number of the legal entity.\",\n      \"$ref\": \"#/components/schemas/PhoneNumber\"\n    },\n    \"principalPlaceOfBusiness\": {\n      \"description\": \"The address where the organization operates from. Provide this if the principal place of business is different from the `registeredAddress`.\",\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"registeredAddress\": {\n      \"description\": \"The address of the organization registered at their registrar (such as the Chamber of Commerce).\",\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"registrationNumber\": {\n      \"description\": \"The organization's registration number.\",\n      \"type\": \"string\"\n    },\n    \"stockData\": {\n      \"description\": \"Information about the organization's publicly traded stock. Provide this object only if `type`\
  \ is **listedPublicCompany**.\",\n      \"$ref\": \"#/components/schemas/StockData\"\n    },\n    \"taxInformation\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The tax information of the organization.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TaxInformation\"\n      },\n      \"type\": \"array\"\n    },\n    \"taxReportingClassification\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The tax reporting classification (FATCA/CRS self-certification) of the organization.\",\n      \"$ref\": \"#/components/schemas/TaxReportingClassification\"\n    },\n    \"type\": {\n      \"description\": \"Type of organization.\\n\\nPossible values: **associationIncorporated**, **governmentalOrganization**, **listedPublicCompany**, **nonProfit**, **partnershipIncorporated**, **privateCompany**.\",\n      \"enum\": [\n        \"associationIncorporated\",\n        \"governmentalOrganization\",\n        \"listedPublicCompany\",\n        \"nonProfit\"\
  ,\n        \"partnershipIncorporated\",\n        \"privateCompany\"\n      ],\n      \"type\": \"string\"\n    },\n    \"vatAbsenceReason\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The reason the organization has not provided a VAT number.\\n\\nPossible values: **industryExemption**, **belowTaxThreshold**.\",\n      \"enum\": [\n        \"industryExemption\",\n        \"belowTaxThreshold\"\n      ],\n      \"type\": \"string\"\n    },\n    \"vatNumber\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The organization's VAT number.\",\n      \"type\": \"string\"\n    },\n    \"webData\": {\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"1\",\n      \"description\": \"The website and app URL of the legal entity.\",\n      \"$ref\": \"#/components/schemas/WebData\"\n    }\n  },\n  \"required\": [\n    \"legalName\",\n    \"registeredAddress\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-organization-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Organization
---
