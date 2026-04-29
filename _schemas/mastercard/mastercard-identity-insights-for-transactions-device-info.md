---
description: This field contains information related to the consumer device used to authorize with your product or service.
layout: schema
name: DeviceInfo
properties_list:
- description: The device type used to authorize your product or service.
  name: deviceType
  type: string
- description: The country where the consumer device is located when attempting to authorize with your product or service.
  name: country
  type: string
- description: The service provider used by the consumer device when attempting to authorize with your product or service.
  name: ipCarrier
  type: string
- description: The city where the consumer device is located when attempting to authorize with your product or service.
  name: city
  type: string
- description: The name of the browser used to authorize your product or service.
  name: browser
  type: string
- description: The state where the consumer device is located when attempting to authorize with your product or service.
  name: state
  type: string
- description: The device platform used to authorize your product or service.
  name: platform
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-identity-insights-for-transactions-device-info-schema.json
slug: mastercard-identity-insights-for-transactions-device-info
source_filename: mastercard-identity-insights-for-transactions-device-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeviceInfo\",\n  \"type\": \"object\",\n  \"description\": \"This field contains information related to the consumer device used to authorize with your product or service.\",\n  \"properties\": {\n    \"deviceType\": {\n      \"type\": \"string\",\n      \"description\": \"The device type used to authorize your product or service.\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"The country where the consumer device is located when attempting to authorize with your product or service.\"\n    },\n    \"ipCarrier\": {\n      \"type\": \"string\",\n      \"description\": \"The service provider used by the consumer device when attempting to authorize with your product or service.\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"The city where the consumer device is located when attempting to authorize with your product or service.\"\
  \n    },\n    \"browser\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the browser used to authorize your product or service.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The state where the consumer device is located when attempting to authorize with your product or service.\"\n    },\n    \"platform\": {\n      \"type\": \"string\",\n      \"description\": \"The device platform used to authorize your product or service.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-identity-insights-for-transactions-device-info-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: DeviceInfo
---
