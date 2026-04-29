---
description: Contact schema from Adyen API
layout: schema
name: Contact
properties_list:
- description: The address of the contact.
  name: address
  type: object
- description: The e-mail address of the contact.
  name: email
  type: string
- description: The phone number of the contact provided as a single string. It will be handled as a landline phone. **Examples:** "0031 6 11 22 33 44", "+316/1122-3344", "(0031) 611223344"
  name: fullPhoneNumber
  type: string
- description: The name of the contact.
  name: name
  type: object
- description: Personal data of the contact.
  name: personalData
  type: object
- description: The phone number of the contact.
  name: phoneNumber
  type: object
- description: The URL of the website of the contact.
  name: webAddress
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-contact-schema.json
slug: notification-webhooks-contact
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-contact-schema.json\",\n  \"title\": \"Contact\",\n  \"description\": \"Contact schema from Adyen API\",\n  \"properties\": {\n    \"address\": {\n      \"description\": \"The address of the contact.\",\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"email\": {\n      \"description\": \"The e-mail address of the contact.\",\n      \"type\": \"string\"\n    },\n    \"fullPhoneNumber\": {\n      \"description\": \"The phone number of the contact provided as a single string.  It will be handled as a landline phone.\\n**Examples:** \\\"0031 6 11 22 33 44\\\", \\\"+316/1122-3344\\\", \\\"(0031) 611223344\\\"\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The name of the contact.\",\n      \"$ref\": \"#/components/schemas/Name\"\n    },\n    \"\
  personalData\": {\n      \"description\": \"Personal data of the contact.\",\n      \"$ref\": \"#/components/schemas/PersonalData\"\n    },\n    \"phoneNumber\": {\n      \"description\": \"The phone number of the contact.\",\n      \"$ref\": \"#/components/schemas/PhoneNumber\"\n    },\n    \"webAddress\": {\n      \"description\": \"The URL of the website of the contact.\",\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-contact-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Contact
---
