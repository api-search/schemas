---
description: A gift card product available through the Reloadly Gift Cards API
layout: schema
name: Reloadly Gift Card Product
properties_list:
- description: Unique product identifier
  name: productId
  type: integer
- description: Display name of the gift card product
  name: productName
  type: string
- description: Whether the product is redeemable globally
  name: global
  type: boolean
- description: Whether pre-ordering is supported
  name: supportsPreOrder
  type: boolean
- description: Fee charged to the sender
  name: senderFee
  type: number
- description: Discount percentage applied to the face value
  name: discountPercentage
  type: number
- description: Whether the product has fixed or range denominations
  name: denominationType
  type: string
- description: ISO 4217 currency code for the recipient
  name: recipientCurrencyCode
  type: string
- description: Minimum denomination for range products
  name: minRecipientDenomination
  type:
  - number
  - 'null'
- description: Maximum denomination for range products
  name: maxRecipientDenomination
  type:
  - number
  - 'null'
- description: ISO 4217 currency code for the sender
  name: senderCurrencyCode
  type: string
- description: Minimum sender denomination for range products
  name: minSenderDenomination
  type:
  - number
  - 'null'
- description: Maximum sender denomination for range products
  name: maxSenderDenomination
  type:
  - number
  - 'null'
- description: Fixed denomination amounts available for the recipient
  name: fixedRecipientDenominations
  type: array
- description: Fixed denomination amounts for the sender
  name: fixedSenderDenominations
  type: array
- description: ''
  name: brand
  type: object
- description: ''
  name: country
  type: object
- description: ''
  name: redeemInstruction
  type: object
provider_name: Reloadly
provider_slug: reloadly
schema_file: json-schema/reloadly-product-schema.json
slug: reloadly-product
source_filename: reloadly-product-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://api-evangelist.github.io/reloadly/json-schema/reloadly-product-schema.json\",\n  \"title\": \"Reloadly Gift Card Product\",\n  \"description\": \"A gift card product available through the Reloadly Gift Cards API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"productId\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique product identifier\"\n    },\n    \"productName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the gift card product\"\n    },\n    \"global\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the product is redeemable globally\"\n    },\n    \"supportsPreOrder\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether pre-ordering is supported\"\n    },\n    \"senderFee\": {\n      \"type\": \"number\",\n      \"description\": \"Fee charged to the sender\"\n    },\n    \"discountPercentage\": {\n\
  \      \"type\": \"number\",\n      \"description\": \"Discount percentage applied to the face value\"\n    },\n    \"denominationType\": {\n      \"type\": \"string\",\n      \"enum\": [\"FIXED\", \"RANGE\"],\n      \"description\": \"Whether the product has fixed or range denominations\"\n    },\n    \"recipientCurrencyCode\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"description\": \"ISO 4217 currency code for the recipient\"\n    },\n    \"minRecipientDenomination\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Minimum denomination for range products\"\n    },\n    \"maxRecipientDenomination\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Maximum denomination for range products\"\n    },\n    \"senderCurrencyCode\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"description\": \"ISO 4217 currency code for the sender\"\n    },\n    \"minSenderDenomination\": {\n      \"type\"\
  : [\"number\", \"null\"],\n      \"description\": \"Minimum sender denomination for range products\"\n    },\n    \"maxSenderDenomination\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Maximum sender denomination for range products\"\n    },\n    \"fixedRecipientDenominations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"number\"\n      },\n      \"description\": \"Fixed denomination amounts available for the recipient\"\n    },\n    \"fixedSenderDenominations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"number\"\n      },\n      \"description\": \"Fixed denomination amounts for the sender\"\n    },\n    \"brand\": {\n      \"$ref\": \"#/$defs/Brand\"\n    },\n    \"country\": {\n      \"$ref\": \"#/$defs/Country\"\n    },\n    \"redeemInstruction\": {\n      \"$ref\": \"#/$defs/RedeemInstruction\"\n    }\n  },\n  \"required\": [\"productId\", \"productName\", \"denominationType\"],\n  \"$defs\": {\n    \"\
  Brand\": {\n      \"type\": \"object\",\n      \"description\": \"Gift card brand information\",\n      \"properties\": {\n        \"brandId\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique brand identifier\"\n        },\n        \"brandName\": {\n          \"type\": \"string\",\n          \"description\": \"Brand display name\"\n        }\n      },\n      \"required\": [\"brandId\", \"brandName\"]\n    },\n    \"Country\": {\n      \"type\": \"object\",\n      \"description\": \"Country information\",\n      \"properties\": {\n        \"isoName\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{2}$\",\n          \"description\": \"ISO 3166-1 alpha-2 country code\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Country display name\"\n        },\n        \"flagUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the country flag image\"\
  \n        }\n      }\n    },\n    \"RedeemInstruction\": {\n      \"type\": \"object\",\n      \"description\": \"Gift card redemption instructions\",\n      \"properties\": {\n        \"concise\": {\n          \"type\": \"string\",\n          \"description\": \"Brief redemption instructions\"\n        },\n        \"verbose\": {\n          \"type\": \"string\",\n          \"description\": \"Detailed redemption instructions\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/reloadly/refs/heads/main/json-schema/reloadly-product-schema.json
tags:
- Gift Cards
- Payments
- Airtime
- Mobile Top-Up
- Rewards
- Incentives
title: Reloadly Gift Card Product
---
