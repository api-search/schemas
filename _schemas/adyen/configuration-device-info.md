---
description: DeviceInfo schema from Adyen API
layout: schema
name: DeviceInfo
properties_list:
- description: The technology used to capture the card details.
  name: cardCaptureTechnology
  type: string
- description: The name of the device.
  name: deviceName
  type: string
- description: The form factor of the device to be provisioned.
  name: formFactor
  type: string
- description: The IMEI number of the device being provisioned.
  name: imei
  type: string
- description: The 2-digit device type provided on the ISO messages that the token is being provisioned to.
  name: isoDeviceType
  type: string
- description: The MSISDN of the device being provisioned.
  name: msisdn
  type: string
- description: The name of the device operating system.
  name: osName
  type: string
- description: The version of the device operating system.
  name: osVersion
  type: string
- description: Different types of payments supported for the network token.
  name: paymentTypes
  type: array
- description: The serial number of the device.
  name: serialNumber
  type: string
- description: The architecture or technology used for network token storage.
  name: storageTechnology
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-device-info-schema.json
slug: configuration-device-info
source_filename: configuration-device-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-device-info-schema.json\",\n  \"title\": \"DeviceInfo\",\n  \"description\": \"DeviceInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cardCaptureTechnology\": {\n      \"description\": \"The technology used to capture the card details.\",\n      \"type\": \"string\"\n    },\n    \"deviceName\": {\n      \"description\": \"The name of the device.\",\n      \"type\": \"string\"\n    },\n    \"formFactor\": {\n      \"description\": \"The form factor of the device to be provisioned.\",\n      \"type\": \"string\"\n    },\n    \"imei\": {\n      \"description\": \"The IMEI number of the device being provisioned.\",\n      \"type\": \"string\"\n    },\n    \"isoDeviceType\": {\n      \"description\": \"The 2-digit device type provided on the ISO messages that the token\
  \ is being provisioned to.\",\n      \"type\": \"string\"\n    },\n    \"msisdn\": {\n      \"description\": \"The MSISDN of the device being provisioned.\",\n      \"type\": \"string\"\n    },\n    \"osName\": {\n      \"description\": \"The name of the device operating system.\",\n      \"type\": \"string\"\n    },\n    \"osVersion\": {\n      \"description\": \"The version of the device operating system.\",\n      \"type\": \"string\"\n    },\n    \"paymentTypes\": {\n      \"description\": \"Different types of payments supported for the network token.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"serialNumber\": {\n      \"description\": \"The serial number of the device.\",\n      \"type\": \"string\"\n    },\n    \"storageTechnology\": {\n      \"description\": \"The architecture or technology used for network token storage.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-device-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DeviceInfo
---
