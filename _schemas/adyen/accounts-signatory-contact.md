---
description: SignatoryContact schema from Adyen API
layout: schema
name: SignatoryContact
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
- description: 'Job title of the signatory. Example values: **Chief Executive Officer**, **Chief Financial Officer**, **Chief Operating Officer**, **President**, **Vice President**, **Executive President**, **Managin'
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
- description: The unique identifier (UUID) of the signatory. >**If, during an Account Holder create or update request, this field is left blank (but other fields provided), a new Signatory will be created with a pr
  name: signatoryCode
  type: string
- description: Your reference for the signatory.
  name: signatoryReference
  type: string
- description: The URL of the person's website.
  name: webAddress
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-signatory-contact-schema.json
slug: accounts-signatory-contact
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-signatory-contact-schema.json\",\n  \"title\": \"SignatoryContact\",\n  \"description\": \"SignatoryContact schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"description\": \"The address of the person.\",\n      \"$ref\": \"#/components/schemas/ViasAddress\"\n    },\n    \"email\": {\n      \"description\": \"The e-mail address of the person.\",\n      \"type\": \"string\"\n    },\n    \"fullPhoneNumber\": {\n      \"description\": \"The phone number of the person provided as a single string.  It will be handled as a landline phone.\\nExamples: \\\"0031 6 11 22 33 44\\\", \\\"+316/1122-3344\\\", \\\"(0031) 611223344\\\"\",\n      \"type\": \"string\"\n    },\n    \"jobTitle\": {\n      \"description\": \"Job title of the signatory.\\n\\nExample values: **Chief\
  \ Executive Officer**, **Chief Financial Officer**, **Chief Operating Officer**, **President**, **Vice President**, **Executive President**, **Managing Member**, **Partner**, **Treasurer**, **Director**, or **Other**.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The name of the person.\",\n      \"$ref\": \"#/components/schemas/ViasName\"\n    },\n    \"personalData\": {\n      \"description\": \"Contains information about the person.\",\n      \"$ref\": \"#/components/schemas/ViasPersonalData\"\n    },\n    \"phoneNumber\": {\n      \"description\": \"The phone number of the person.\",\n      \"$ref\": \"#/components/schemas/ViasPhoneNumber\"\n    },\n    \"signatoryCode\": {\n      \"description\": \"The unique identifier (UUID) of the signatory.\\n>**If, during an Account Holder create or update request, this field is left blank (but other fields provided), a new Signatory will be created with a procedurally-generated UUID.**\\n\\n>**If, during an\
  \ Account Holder create request, a UUID is provided, the creation of the Signatory will fail while the creation of the Account Holder will continue.**\\n\\n>**If, during an Account Holder update request, a UUID that is not correlated with an existing Signatory is provided, the update of the Signatory will fail.**\\n\\n>**If, during an Account Holder update request, a UUID that is correlated with an existing Signatory is provided, the existing Signatory will be updated.**\\n\",\n      \"type\": \"string\"\n    },\n    \"signatoryReference\": {\n      \"description\": \"Your reference for the signatory.\",\n      \"type\": \"string\"\n    },\n    \"webAddress\": {\n      \"description\": \"The URL of the person's website.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-signatory-contact-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SignatoryContact
---
