---
description: BrowserInfo schema from Adyen API
layout: schema
name: BrowserInfo
properties_list:
- description: The accept header value of the shopper's browser.
  name: acceptHeader
  type: string
- description: 'The color depth of the shopper''s browser in bits per pixel. This should be obtained by using the browser''s `screen.colorDepth` property. Accepted values: 1, 4, 8, 15, 16, 24, 30, 32 or 48 bit color de'
  name: colorDepth
  type: integer
- description: Boolean value indicating if the shopper's browser is able to execute Java.
  name: javaEnabled
  type: boolean
- description: Boolean value indicating if the shopper's browser is able to execute JavaScript. A default 'true' value is assumed if the field is not present.
  name: javaScriptEnabled
  type: boolean
- description: The `navigator.language` value of the shopper's browser (as defined in IETF BCP 47).
  name: language
  type: string
- description: The total height of the shopper's device screen in pixels.
  name: screenHeight
  type: integer
- description: The total width of the shopper's device screen in pixels.
  name: screenWidth
  type: integer
- description: Time difference between UTC time and the shopper's browser local time, in minutes.
  name: timeZoneOffset
  type: integer
- description: The user agent value of the shopper's browser.
  name: userAgent
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-browser-info-schema.json
slug: checkout-browser-info
source_filename: checkout-browser-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-browser-info-schema.json\",\n  \"title\": \"BrowserInfo\",\n  \"description\": \"BrowserInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"acceptHeader\": {\n      \"description\": \"The accept header value of the shopper's browser.\",\n      \"type\": \"string\"\n    },\n    \"colorDepth\": {\n      \"x-addedInVersion\": \"40\",\n      \"description\": \"The color depth of the shopper's browser in bits per pixel. This should be obtained by using the browser's `screen.colorDepth` property. Accepted values: 1, 4, 8, 15, 16, 24, 30, 32 or 48 bit color depth.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"javaEnabled\": {\n      \"x-addedInVersion\": \"40\",\n      \"description\": \"Boolean value indicating if the shopper's browser is able to execute\
  \ Java.\",\n      \"type\": \"boolean\"\n    },\n    \"javaScriptEnabled\": {\n      \"x-addedInVersion\": \"40\",\n      \"default\": true,\n      \"description\": \"Boolean value indicating if the shopper's browser is able to execute JavaScript. A default 'true' value is assumed if the field is not present.\",\n      \"type\": \"boolean\"\n    },\n    \"language\": {\n      \"x-addedInVersion\": \"40\",\n      \"description\": \"The `navigator.language` value of the shopper's browser (as defined in IETF BCP 47).\",\n      \"type\": \"string\"\n    },\n    \"screenHeight\": {\n      \"x-addedInVersion\": \"40\",\n      \"description\": \"The total height of the shopper's device screen in pixels.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"screenWidth\": {\n      \"x-addedInVersion\": \"40\",\n      \"description\": \"The total width of the shopper's device screen in pixels.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"timeZoneOffset\"\
  : {\n      \"x-addedInVersion\": \"40\",\n      \"description\": \"Time difference between UTC time and the shopper's browser local time, in minutes.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"userAgent\": {\n      \"description\": \"The user agent value of the shopper's browser.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"userAgent\",\n    \"acceptHeader\",\n    \"javaEnabled\",\n    \"colorDepth\",\n    \"screenHeight\",\n    \"screenWidth\",\n    \"timeZoneOffset\",\n    \"language\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-browser-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BrowserInfo
---
