---
description: Document schema from Adyen API
layout: schema
name: Document
properties_list:
- description: Object that contains the document.
  name: attachment
  type: object
- description: Array that contains the document. The array supports multiple attachments for uploading different sides or pages of a document.
  name: attachments
  type: array
- description: The creation date of the document.
  name: creationDate
  type: string
- description: Your description for the document.
  name: description
  type: string
- description: The expiry date of the document, in YYYY-MM-DD format.
  name: expiryDate
  type: string
- description: The filename of the document.
  name: fileName
  type: string
- description: The unique identifier of the document.
  name: id
  type: string
- description: The two-character [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) country code where the document was issued. For example, **US**.
  name: issuerCountry
  type: string
- description: The state or province where the document was issued (AU only).
  name: issuerState
  type: string
- description: The modification date of the document.
  name: modificationDate
  type: string
- description: The number in the document.
  name: number
  type: string
- description: Contains information about the resource that owns the document.
  name: owner
  type: object
- description: Type of document, used when providing an ID number or uploading a document. The possible values depend on the legal entity type. * For **organization**, the `type` values can be **proofOfAddress**, **
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-document-schema.json
slug: legal-entity-document
source_filename: legal-entity-document-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-document-schema.json\",\n  \"title\": \"Document\",\n  \"description\": \"Document schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attachment\": {\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"1\",\n      \"x-deprecatedMessage\": \"Use the `attachments` array instead.\",\n      \"description\": \"Object that contains the document.\",\n      \"$ref\": \"#/components/schemas/Attachment\"\n    },\n    \"attachments\": {\n      \"description\": \"Array that contains the document. The array supports multiple attachments for uploading different sides or pages of a document.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Attachment\"\n      },\n      \"type\": \"array\"\n    },\n    \"creationDate\": {\n      \"description\": \"The creation\
  \ date of the document.\",\n      \"format\": \"date-time\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"description\": \"Your description for the document.\",\n      \"type\": \"string\"\n    },\n    \"expiryDate\": {\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"1\",\n      \"description\": \"The expiry date of the document, in YYYY-MM-DD format.\",\n      \"type\": \"string\"\n    },\n    \"fileName\": {\n      \"description\": \"The filename of the document.\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the document.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"issuerCountry\": {\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"1\",\n      \"description\": \"The two-character [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) country code where the document was issued. For example, **US**.\"\
  ,\n      \"type\": \"string\"\n    },\n    \"issuerState\": {\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"1\",\n      \"description\": \"The state or province where the document was issued (AU only).\",\n      \"type\": \"string\"\n    },\n    \"modificationDate\": {\n      \"description\": \"The modification date of the document.\",\n      \"format\": \"date-time\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"number\": {\n      \"description\": \"The number in the document.\",\n      \"type\": \"string\"\n    },\n    \"owner\": {\n      \"description\": \"Contains information about the resource that owns the document.\",\n      \"$ref\": \"#/components/schemas/OwnerEntity\"\n    },\n    \"type\": {\n      \"description\": \"Type of document, used when providing an ID number or uploading a document. The possible values depend on the legal entity type.\\n\\n* For **organization**, the `type` values can be **proofOfAddress**, **registrationDocument**,\
  \ **vatDocument**, **proofOfOrganizationTaxInfo**, **proofOfOwnership**, **proofOfIndustry**, or **proofOfFundingOrWealthSource**.\\n\\n* For **individual**, the `type` values can be **identityCard**, **driversLicense**, **passport**, **proofOfNationalIdNumber**, **proofOfResidency**, **proofOfIndustry**, **proofOfIndividualTaxId**, or **proofOfFundingOrWealthSource**.\\n\\n* For **soleProprietorship**, the `type` values can be **constitutionalDocument**, **proofOfAddress**, or **proofOfIndustry**.\\n\\n* Use **bankStatement** to upload documents for a [transfer instrument](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/transferInstruments__resParam_id).\",\n      \"enum\": [\n        \"bankStatement\",\n        \"driversLicense\",\n        \"identityCard\",\n        \"nationalIdNumber\",\n        \"passport\",\n        \"proofOfAddress\",\n        \"proofOfNationalIdNumber\",\n        \"proofOfResidency\",\n        \"registrationDocument\",\n        \"vatDocument\",\n \
  \       \"proofOfOrganizationTaxInfo\",\n        \"proofOfIndustry\",\n        \"constitutionalDocument\",\n        \"proofOfFundingOrWealthSource\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"description\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-document-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Document
---
