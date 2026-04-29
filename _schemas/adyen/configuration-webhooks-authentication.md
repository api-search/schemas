---
description: Authentication schema from Adyen API
layout: schema
name: Authentication
properties_list:
- description: The email address where the one-time password (OTP) is sent.
  name: email
  type: string
- description: The password used for 3D Secure password-based authentication. The value must be between 1 to 30 characters and must only contain the following supported characters. * Characters between **a-z**, **A-
  name: password
  type: string
- description: 'The phone number where the one-time password (OTP) is sent. This object must have: * A `type` set to **mobile**. * A `number` with a valid country code. * A `number` with more than 4 digits, excluding'
  name: phone
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-webhooks-authentication-schema.json
slug: configuration-webhooks-authentication
source_filename: configuration-webhooks-authentication-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-authentication-schema.json\",\n  \"title\": \"Authentication\",\n  \"description\": \"Authentication schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"email\": {\n      \"description\": \"The email address where the one-time password (OTP) is sent.\",\n      \"type\": \"string\"\n    },\n    \"password\": {\n      \"description\": \"The password used for 3D Secure password-based authentication. The value must be between 1 to 30 characters and must only contain the following supported characters.\\n\\n* Characters between **a-z**, **A-Z**, and **0-9**\\n\\n* Special characters: **\\u00e4\\u00f6\\u00fc\\u00df\\u00c4\\u00d6\\u00dc+-*/\\u00e7%()=?!~#'\\\",;:$&\\u00e0\\u00f9\\u00f2\\u00e2\\u00f4\\u00fb\\u00e1\\u00fa\\u00f3**\",\n      \"maxLength\": 30,\n      \"minLength\"\
  : 1,\n      \"type\": \"string\"\n    },\n    \"phone\": {\n      \"description\": \"The phone number where the one-time password (OTP) is sent.\\n\\nThis object must have:\\n\\n* A `type` set to **mobile**.\\n\\n* A `number` with a valid country code.\\n\\n* A `number` with more than 4 digits, excluding the country code.\\n\\n>Make sure to verify that the card user owns the phone number.\",\n      \"$ref\": \"#/components/schemas/Phone\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-authentication-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Authentication
---
