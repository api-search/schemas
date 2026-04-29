---
description: TaxReportingClassification schema from Adyen API
layout: schema
name: TaxReportingClassification
properties_list:
- description: 'The organization''s business type. Possible values: **other**, **listedPublicCompany**, **subsidiaryOfListedPublicCompany**, **governmentalOrganization**, **internationalOrganization**, **financialInst'
  name: businessType
  type: string
- description: The Global Intermediary Identification Number (GIIN) required for FATCA. Only required if the organization is a US financial institution and the `businessType` is **financialInstitution**.
  name: financialInstitutionNumber
  type: string
- description: 'The organization''s main source of income. Possible values: **businessOperation**, **realEstateSales**, **investmentInterestOrRoyalty**, **propertyRental**, **other**.'
  name: mainSourceOfIncome
  type: string
- description: 'The tax reporting classification type. Possible values: **nonFinancialNonReportable**, **financialNonReportable**, **nonFinancialActive**, **nonFinancialPassive**.'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-tax-reporting-classification-schema.json
slug: legal-entity-tax-reporting-classification
source_filename: legal-entity-tax-reporting-classification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-tax-reporting-classification-schema.json\",\n  \"title\": \"TaxReportingClassification\",\n  \"description\": \"TaxReportingClassification schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"businessType\": {\n      \"description\": \"The organization's business type.\\n\\nPossible values: **other**, **listedPublicCompany**, **subsidiaryOfListedPublicCompany**, **governmentalOrganization**, **internationalOrganization**, **financialInstitution**.\",\n      \"enum\": [\n        \"other\",\n        \"listedPublicCompany\",\n        \"subsidiaryOfListedPublicCompany\",\n        \"governmentalOrganization\",\n        \"internationalOrganization\",\n        \"financialInstitution.\"\n      ],\n      \"type\": \"string\"\n    },\n    \"financialInstitutionNumber\": {\n      \"description\"\
  : \"The Global Intermediary Identification Number (GIIN) required for FATCA. Only required if the organization is a US financial institution and the `businessType` is **financialInstitution**.\",\n      \"type\": \"string\"\n    },\n    \"mainSourceOfIncome\": {\n      \"description\": \"The organization's main source of income.\\n\\nPossible values: **businessOperation**, **realEstateSales**, **investmentInterestOrRoyalty**, **propertyRental**, **other**.\",\n      \"enum\": [\n        \"businessOperation\",\n        \"realEstateSales\",\n        \"investmentInterestOrRoyalty\",\n        \"propertyRental\",\n        \"other\"\n      ],\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The tax reporting classification type.\\n\\nPossible values: **nonFinancialNonReportable**, **financialNonReportable**, **nonFinancialActive**, **nonFinancialPassive**.\",\n      \"enum\": [\n        \"nonFinancialNonReportable\",\n        \"financialNonReportable\",\n      \
  \  \"nonFinancialActive\",\n        \"nonFinancialPassive\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-tax-reporting-classification-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TaxReportingClassification
---
