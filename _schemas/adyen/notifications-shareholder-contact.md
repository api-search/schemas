---
description: ShareholderContact schema from Adyen API
layout: schema
name: ShareholderContact
properties_list:
- description: The address of the person.
  name: address
  type: object
- description: The e-mail address of the person.
  name: email
  type: string
- description: 'The phone number of the person provided as a single string. It will be handled as a landline phone. Examples: "0031 6 11 22 33 44", "+316/1122-3344", "(0031) 611223344"'
  name: fullPhoneNumber
  type: string
- description: 'Job title of the person. Required when the `shareholderType` is **Controller**. Example values: **Chief Executive Officer**, **Chief Financial Officer**, **Chief Operating Officer**, **President**, **'
  name: jobTitle
  type: string
- description: The name of the person.
  name: name
  type: object
- description: Contains information about the person.
  name: personalData
  type: object
- description: The phone number of the person.
  name: phoneNumber
  type: object
- description: The unique identifier (UUID) of the shareholder entry. >**If, during an Account Holder create or update request, this field is left blank (but other fields provided), a new Shareholder will be created
  name: shareholderCode
  type: string
- description: Your reference for the shareholder entry.
  name: shareholderReference
  type: string
- description: 'Specifies how the person is associated with the account holder. Possible values: * **Owner**: Individuals who directly or indirectly own 25% or more of a company. * **Controller**: Individuals who are'
  name: shareholderType
  type: string
- description: The URL of the person's website.
  name: webAddress
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-shareholder-contact-schema.json
slug: notifications-shareholder-contact
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-shareholder-contact-schema.json\",\n  \"title\": \"ShareholderContact\",\n  \"description\": \"ShareholderContact schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"description\": \"The address of the person.\",\n      \"$ref\": \"#/components/schemas/ViasAddress\"\n    },\n    \"email\": {\n      \"description\": \"The e-mail address of the person.\",\n      \"type\": \"string\"\n    },\n    \"fullPhoneNumber\": {\n      \"description\": \"The phone number of the person provided as a single string.  It will be handled as a landline phone.\\nExamples: \\\"0031 6 11 22 33 44\\\", \\\"+316/1122-3344\\\", \\\"(0031) 611223344\\\"\",\n      \"type\": \"string\"\n    },\n    \"jobTitle\": {\n      \"description\": \"Job title of the person. Required when\
  \ the `shareholderType` is **Controller**.\\n\\nExample values: **Chief Executive Officer**, **Chief Financial Officer**, **Chief Operating Officer**, **President**, **Vice President**, **Executive President**, **Managing Member**, **Partner**, **Treasurer**, **Director**, or **Other**.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The name of the person.\",\n      \"$ref\": \"#/components/schemas/ViasName\"\n    },\n    \"personalData\": {\n      \"description\": \"Contains information about the person.\",\n      \"$ref\": \"#/components/schemas/ViasPersonalData\"\n    },\n    \"phoneNumber\": {\n      \"description\": \"The phone number of the person.\",\n      \"$ref\": \"#/components/schemas/ViasPhoneNumber\"\n    },\n    \"shareholderCode\": {\n      \"description\": \"The unique identifier (UUID) of the shareholder entry.\\n>**If, during an Account Holder create or update request, this field is left blank (but other fields provided), a new Shareholder\
  \ will be created with a procedurally-generated UUID.**\\n\\n>**If, during an Account Holder create request, a UUID is provided, the creation of Account Holder will fail with a validation Error..**\\n\\n>**If, during an Account Holder update request, a UUID that is not correlated with an existing Shareholder is provided, the update of the Shareholder will fail.**\\n\\n>**If, during an Account Holder update request, a UUID that is correlated with an existing Shareholder is provided, the existing Shareholder will be updated.**\\n\",\n      \"type\": \"string\"\n    },\n    \"shareholderReference\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"Your reference for the shareholder entry.\",\n      \"type\": \"string\"\n    },\n    \"shareholderType\": {\n      \"description\": \"Specifies how the person is associated with the account holder. \\n\\nPossible values: \\n\\n* **Owner**: Individuals who directly or indirectly own 25% or more of a company.\\n\\n* **Controller**:\
  \ Individuals who are members of senior management staff responsible for managing a company or organization.\",\n      \"enum\": [\n        \"Controller\",\n        \"Owner\",\n        \"Signatory\"\n      ],\n      \"type\": \"string\"\n    },\n    \"webAddress\": {\n      \"description\": \"The URL of the person's website.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-shareholder-contact-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ShareholderContact
---
