---
description: ContactDetails schema from Adyen API
layout: schema
name: ContactDetails
properties_list:
- description: The address of the account holder.
  name: address
  type: object
- description: The email address of the account holder.
  name: email
  type: string
- description: The phone number of the account holder.
  name: phone
  type: object
- description: The URL of the account holder's website.
  name: webAddress
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-contact-details-schema.json
slug: notification-webhooks-contact-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-contact-details-schema.json\",\n  \"title\": \"ContactDetails\",\n  \"description\": \"ContactDetails schema from Adyen API\",\n  \"properties\": {\n    \"address\": {\n      \"description\": \"The address of the account holder.\",\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"email\": {\n      \"description\": \"The email address of the account holder.\",\n      \"type\": \"string\"\n    },\n    \"phone\": {\n      \"description\": \"The phone number of the account holder.\",\n      \"$ref\": \"#/components/schemas/Phone\"\n    },\n    \"webAddress\": {\n      \"description\": \"The URL of the account holder's website.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"email\",\n    \"phone\",\n    \"address\"\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-contact-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ContactDetails
---
