---
description: LegalArrangementEntityDetail schema from Adyen API
layout: schema
name: LegalArrangementEntityDetail
properties_list:
- description: The address of the entity.
  name: address
  type: object
- description: Required when creating an entity with `legalEntityType` **Business**, **NonProfit**, **PublicCompany**, or **Partnership**.
  name: businessDetails
  type: object
- description: The e-mail address of the entity.
  name: email
  type: string
- description: The phone number of the contact provided as a single string. It will be handled as a landline phone. **Examples:** "0031 6 11 22 33 44", "+316/1122-3344", "(0031) 611223344"
  name: fullPhoneNumber
  type: string
- description: Required when creating an entity with `legalEntityType` **Individual**.
  name: individualDetails
  type: object
- description: 'Adyen-generated unique alphanumeric identifier (UUID) for the entry, returned in the response when you create a legal arrangement entity. Use only when updating an account holder. If you include this '
  name: legalArrangementEntityCode
  type: string
- description: Your reference for the legal arrangement entity.
  name: legalArrangementEntityReference
  type: string
- description: 'An array containing the roles of the entity in the legal arrangement. The possible values depend on the legal arrangement `type`. - For `type` **Association**: **ControllingPerson** and **Shareholder*'
  name: legalArrangementMembers
  type: array
- description: 'The legal entity type. Possible values: **Business**, **Individual**, **NonProfit**, **PublicCompany**, or **Partnership**.'
  name: legalEntityType
  type: string
- description: The phone number of the entity.
  name: phoneNumber
  type: object
- description: The URL of the website of the contact.
  name: webAddress
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-legal-arrangement-entity-detail-schema.json
slug: accounts-legal-arrangement-entity-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-legal-arrangement-entity-detail-schema.json\",\n  \"title\": \"LegalArrangementEntityDetail\",\n  \"description\": \"LegalArrangementEntityDetail schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"description\": \"The address of the entity.\",\n      \"$ref\": \"#/components/schemas/ViasAddress\"\n    },\n    \"businessDetails\": {\n      \"description\": \"Required when creating an entity with `legalEntityType` **Business**, **NonProfit**, **PublicCompany**, or **Partnership**.\",\n      \"$ref\": \"#/components/schemas/BusinessDetails\"\n    },\n    \"email\": {\n      \"description\": \"The e-mail address of the entity.\",\n      \"type\": \"string\"\n    },\n    \"fullPhoneNumber\": {\n      \"description\": \"The phone number of the contact provided\
  \ as a single string.  It will be handled as a landline phone.\\n**Examples:** \\\"0031 6 11 22 33 44\\\", \\\"+316/1122-3344\\\", \\\"(0031) 611223344\\\"\",\n      \"type\": \"string\"\n    },\n    \"individualDetails\": {\n      \"description\": \"Required when creating an entity with `legalEntityType` **Individual**.\",\n      \"$ref\": \"#/components/schemas/IndividualDetails\"\n    },\n    \"legalArrangementEntityCode\": {\n      \"description\": \"Adyen-generated unique alphanumeric identifier (UUID) for the entry, returned in the response when you create a legal arrangement entity.\\nUse only when updating an account holder. If you include this field when creating an account holder, the request will fail.\",\n      \"type\": \"string\"\n    },\n    \"legalArrangementEntityReference\": {\n      \"description\": \"Your reference for the legal arrangement entity.\",\n      \"type\": \"string\"\n    },\n    \"legalArrangementMembers\": {\n      \"description\": \"An array containing\
  \ the roles of the entity in the legal arrangement.\\n\\nThe possible values depend on the legal arrangement `type`.\\n\\n- For `type` **Association**: **ControllingPerson** and **Shareholder**.\\n\\n- For `type` **Partnership**: **Partner** and **Shareholder**.\\n\\n- For `type` **Trust**: **Trustee**, **Settlor**, **Protector**, **Beneficiary**,  and **Shareholder**.\\n\\n\",\n      \"items\": {\n        \"enum\": [\n          \"Beneficiary\",\n          \"ControllingPerson\",\n          \"Partner\",\n          \"Protector\",\n          \"Settlor\",\n          \"Shareholder\",\n          \"Trustee\"\n        ],\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"legalEntityType\": {\n      \"description\": \"The legal entity type.\\n\\nPossible values: **Business**, **Individual**, **NonProfit**, **PublicCompany**, or **Partnership**. \",\n      \"enum\": [\n        \"Business\",\n        \"Individual\",\n        \"NonProfit\",\n        \"Partnership\",\n\
  \        \"PublicCompany\"\n      ],\n      \"type\": \"string\"\n    },\n    \"phoneNumber\": {\n      \"description\": \"The phone number of the entity.\",\n      \"$ref\": \"#/components/schemas/ViasPhoneNumber\"\n    },\n    \"webAddress\": {\n      \"description\": \"The URL of the website of the contact.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-legal-arrangement-entity-detail-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: LegalArrangementEntityDetail
---
