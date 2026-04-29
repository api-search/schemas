---
description: CardConfiguration schema from Adyen API
layout: schema
name: CardConfiguration
properties_list:
- description: Overrides the activation label design ID defined in the `configurationProfileId`. The activation label is attached to the card and contains the activation instructions.
  name: activation
  type: string
- description: Your app's URL, if you want to activate cards through your app. For example, **my-app://ref1236a7d**. A QR code is created based on this URL, and is included in the carrier. Before you use this field,
  name: activationUrl
  type: string
- description: Overrides the shipment bulk address defined in the `configurationProfileId`.
  name: bulkAddress
  type: object
- description: The ID of the card image. This is the image that will be printed on the full front of the card.
  name: cardImageId
  type: string
- description: Overrides the carrier design ID defined in the `configurationProfileId`. The carrier is the letter or packaging to which the card is attached.
  name: carrier
  type: string
- description: The ID of the carrier image. This is the image that will printed on the letter to which the card is attached.
  name: carrierImageId
  type: string
- description: The ID of the card configuration profile that contains the settings of the card. For example, the envelope and PIN mailer designs or the logistics company handling the shipment. All the settings in th
  name: configurationProfileId
  type: string
- description: The three-letter [ISO-4217](https://en.wikipedia.org/wiki/ISO_4217) currency code of the card. For example, **EUR**.
  name: currency
  type: string
- description: Overrides the envelope design ID defined in the `configurationProfileId`.
  name: envelope
  type: string
- description: Overrides the insert design ID defined in the `configurationProfileId`. An insert is any additional material, such as marketing materials, that are shipped together with the card.
  name: insert
  type: string
- description: The two-letter [ISO-639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) language code of the card. For example, **en**.
  name: language
  type: string
- description: The ID of the logo image. This is the image that will be printed on the partial front of the card, such as a logo on the upper right corner.
  name: logoImageId
  type: string
- description: Overrides the PIN mailer design ID defined in the `configurationProfileId`. The PIN mailer is the letter on which the PIN is printed.
  name: pinMailer
  type: string
- description: Overrides the logistics company defined in the `configurationProfileId`.
  name: shipmentMethod
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-webhooks-card-configuration-schema.json
slug: configuration-webhooks-card-configuration
source_filename: configuration-webhooks-card-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-card-configuration-schema.json\",\n  \"title\": \"CardConfiguration\",\n  \"description\": \"CardConfiguration schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"activation\": {\n      \"description\": \"Overrides the activation label design ID defined in the `configurationProfileId`. The activation label is attached to the card and contains the activation instructions.\",\n      \"type\": \"string\"\n    },\n    \"activationUrl\": {\n      \"description\": \"Your app's URL, if you want to activate cards through your app. For example, **my-app://ref1236a7d**. A QR code is created based on this URL, and is included in the carrier. Before you use this field, reach out to your Adyen contact to set up the QR code process. \\n\\nMaximum length: 255 characters.\",\n  \
  \    \"maxLength\": 255,\n      \"type\": \"string\"\n    },\n    \"bulkAddress\": {\n      \"description\": \"Overrides the shipment bulk address defined in the `configurationProfileId`.\",\n      \"$ref\": \"#/components/schemas/BulkAddress\"\n    },\n    \"cardImageId\": {\n      \"description\": \"The ID of the card image. This is the image that will be printed on the full front of the card.\",\n      \"type\": \"string\"\n    },\n    \"carrier\": {\n      \"description\": \"Overrides the carrier design ID defined in the `configurationProfileId`. The carrier is the letter or packaging to which the card is attached.\",\n      \"type\": \"string\"\n    },\n    \"carrierImageId\": {\n      \"description\": \"The ID of the carrier image. This is the image that will printed on the letter to which the card is attached.\",\n      \"type\": \"string\"\n    },\n    \"configurationProfileId\": {\n      \"description\": \"The ID of the card configuration profile that contains the settings of\
  \ the card. For example, the envelope and PIN mailer designs or the logistics company handling the shipment. All the settings in the profile are applied to the card, unless you provide other fields to override them.\\n\\nFor example, send the `shipmentMethod` to override the logistics company defined in the card configuration profile.\",\n      \"type\": \"string\"\n    },\n    \"currency\": {\n      \"description\": \"The three-letter [ISO-4217](https://en.wikipedia.org/wiki/ISO_4217) currency code of the card. For example, **EUR**.\",\n      \"type\": \"string\"\n    },\n    \"envelope\": {\n      \"description\": \"Overrides the envelope design ID defined in the `configurationProfileId`. \",\n      \"type\": \"string\"\n    },\n    \"insert\": {\n      \"description\": \"Overrides the insert design ID defined in the `configurationProfileId`. An insert is any additional material, such as marketing materials, that are shipped together with the card.\",\n      \"type\": \"string\"\n  \
  \  },\n    \"language\": {\n      \"description\": \"The two-letter [ISO-639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) language code of the card. For example, **en**.\",\n      \"type\": \"string\"\n    },\n    \"logoImageId\": {\n      \"description\": \"The ID of the logo image. This is the image that will be printed on the partial front of the card, such as a logo on the upper right corner.\",\n      \"type\": \"string\"\n    },\n    \"pinMailer\": {\n      \"description\": \"Overrides the PIN mailer design ID defined in the `configurationProfileId`. The PIN mailer is the letter on which the PIN is printed.\",\n      \"type\": \"string\"\n    },\n    \"shipmentMethod\": {\n      \"description\": \"Overrides the logistics company defined in the `configurationProfileId`.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"configurationProfileId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-card-configuration-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CardConfiguration
---
