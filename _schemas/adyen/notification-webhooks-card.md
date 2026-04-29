---
description: Card schema from Adyen API
layout: schema
name: Card
properties_list:
- description: Contains the card user's password and mobile phone number. This is required when you issue cards that can be used to make online payments within the EEA and the UK, or can be added to digital wallets.
  name: authentication
  type: object
- description: The bank identification number (BIN) of the card number.
  name: bin
  type: string
- description: 'The brand of the payment instrument. Possible values: **visa**, **mc**.'
  name: brand
  type: string
- description: 'The brand variant of the payment instrument. >Contact your Adyen Implementation Manager to get the values that are relevant to your integration. Examples: **visadebit**, **mcprepaid**.'
  name: brandVariant
  type: string
- description: 'The name of the cardholder. Maximum length: 26 characters.'
  name: cardholderName
  type: string
- description: Settings required when creating a physical card. Reach out to your Adyen contact to get the values that you can send in this object.
  name: configuration
  type: object
- description: The CVC2 value of the card. > The CVC2 is not sent by default. This is only returned in the `POST` response for single-use virtual cards.
  name: cvc
  type: string
- description: The delivery contact (name and address) for physical card delivery.
  name: deliveryContact
  type: object
- description: The expiration date of the card.
  name: expiration
  type: object
- description: 'The form factor of the card. Possible values: **virtual**, **physical**.'
  name: formFactor
  type: string
- description: Last last four digits of the card number.
  name: lastFour
  type: string
- description: The primary account number (PAN) of the card. > The PAN is masked by default and returned only for single-use virtual cards.
  name: number
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-card-schema.json
slug: notification-webhooks-card
source_filename: notification-webhooks-card-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-card-schema.json\",\n  \"title\": \"Card\",\n  \"description\": \"Card schema from Adyen API\",\n  \"properties\": {\n    \"authentication\": {\n      \"description\": \"Contains the card user's password and mobile phone number. This is required when you issue cards that can be used to make online payments within the EEA and the UK, or can be added to digital wallets. Refer to [3D Secure and digital wallets](https://docs.adyen.com/issuing/3d-secure-and-wallets) for more information.\",\n      \"$ref\": \"#/components/schemas/Authentication\"\n    },\n    \"bin\": {\n      \"description\": \"The bank identification number (BIN) of the card number.\",\n      \"type\": \"string\"\n    },\n    \"brand\": {\n      \"description\": \"The brand of the payment instrument.\\nPossible values: **visa**,\
  \ **mc**.\",\n      \"type\": \"string\"\n    },\n    \"brandVariant\": {\n      \"description\": \"The brand variant of the payment instrument.\\n>Contact your Adyen Implementation Manager to get the values that are relevant to your integration. Examples: **visadebit**, **mcprepaid**.\",\n      \"type\": \"string\"\n    },\n    \"cardholderName\": {\n      \"description\": \"The name of the cardholder.\\n Maximum length: 26 characters.\",\n      \"maxLength\": 26,\n      \"type\": \"string\"\n    },\n    \"configuration\": {\n      \"description\": \"Settings required when creating a physical card. \\n\\nReach out to your Adyen contact to get the values that you can send in this object.\",\n      \"$ref\": \"#/components/schemas/CardConfiguration\"\n    },\n    \"cvc\": {\n      \"description\": \"The CVC2 value of the card.\\n> The CVC2 is not sent by default. This is only returned in the `POST` response for single-use virtual cards.\",\n      \"type\": \"string\"\n    },\n    \"deliveryContact\"\
  : {\n      \"description\": \"The delivery contact (name and address) for physical card delivery.\",\n      \"$ref\": \"#/components/schemas/Contact\"\n    },\n    \"expiration\": {\n      \"description\": \"The expiration date of the card.\",\n      \"$ref\": \"#/components/schemas/Expiry\"\n    },\n    \"formFactor\": {\n      \"description\": \"The form factor of the card.\\nPossible values: **virtual**, **physical**.\",\n      \"enum\": [\n        \"physical\",\n        \"unknown\",\n        \"virtual\"\n      ],\n      \"type\": \"string\"\n    },\n    \"lastFour\": {\n      \"description\": \"Last last four digits of the card number.\",\n      \"type\": \"string\"\n    },\n    \"number\": {\n      \"description\": \"The primary account number (PAN) of the card.\\n> The PAN is masked by default and returned only for single-use virtual cards.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"formFactor\",\n    \"cardholderName\",\n    \"brand\",\n    \"brandVariant\"\
  ,\n    \"number\"\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-card-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Card
---
