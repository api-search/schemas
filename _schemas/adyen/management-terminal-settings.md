---
description: TerminalSettings schema from Adyen API
layout: schema
name: TerminalSettings
properties_list:
- description: Settings to define the header of the shopper receipt.
  name: cardholderReceipt
  type: object
- description: Settings for terminal connectivity features.
  name: connectivity
  type: object
- description: Settings for tipping with or without predefined options to choose from. The maximum number of predefined options is four, or three plus the option to enter a custom tip.
  name: gratuities
  type: array
- description: Settings for terminal hardware features.
  name: hardware
  type: object
- description: Settings for localization.
  name: localization
  type: object
- description: Settings for a Terminal API integration.
  name: nexo
  type: object
- description: Settings for [offline payment](https://docs.adyen.com/point-of-sale/offline-payments) features.
  name: offlineProcessing
  type: object
- description: Settings for an Oracle Payment Interface (OPI) integration.
  name: opi
  type: object
- description: Settings for [passcodes](https://docs.adyen.com/point-of-sale/managing-terminals/menu-access?tab=manage_passcodes_with_an_api_call_2#manage-passcodes) features.
  name: passcodes
  type: object
- description: Settings for [Pay-at-table](https://docs.adyen.com/point-of-sale/pay-at-x) features.
  name: payAtTable
  type: object
- description: Settings for payment features.
  name: payment
  type: object
- description: Generic receipt settings.
  name: receiptOptions
  type: object
- description: Transaction outcomes that you want the terminal to print a merchant receipt or a shopper receipt for.
  name: receiptPrinting
  type: object
- description: Settings for refunds.
  name: refunds
  type: object
- description: Settings to skip signature, sign on display, or sign on receipt.
  name: signature
  type: object
- description: Settings for [standalone](https://docs.adyen.com/point-of-sale/standalone/standalone-build/set-up-standalone#set-up-standalone-using-an-api-call) features.
  name: standalone
  type: object
- description: Settings for payment [surcharge](https://docs.adyen.com/point-of-sale/surcharge) features.
  name: surcharge
  type: object
- description: Settings for Tap to Pay.
  name: tapToPay
  type: object
- description: Settings for device [time-outs](https://docs.adyen.com/point-of-sale/pos-timeouts#device-time-out).
  name: timeouts
  type: object
- description: Remote Wi-Fi profiles for WPA and WPA2 PSK and EAP Wi-Fi networks.
  name: wifiProfiles
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-terminal-settings-schema.json
slug: management-terminal-settings
source_filename: management-terminal-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-settings-schema.json\",\n  \"title\": \"TerminalSettings\",\n  \"description\": \"TerminalSettings schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cardholderReceipt\": {\n      \"description\": \"Settings to define the header of the shopper receipt.\",\n      \"$ref\": \"#/components/schemas/CardholderReceipt\"\n    },\n    \"connectivity\": {\n      \"description\": \"Settings for terminal connectivity features.\",\n      \"$ref\": \"#/components/schemas/Connectivity\"\n    },\n    \"gratuities\": {\n      \"description\": \"Settings for tipping with or without predefined options to choose from. The maximum number of predefined options is four, or three plus the option to enter a custom tip.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Gratuity\"\
  \n      },\n      \"type\": \"array\"\n    },\n    \"hardware\": {\n      \"description\": \"Settings for terminal hardware features.\",\n      \"$ref\": \"#/components/schemas/Hardware\"\n    },\n    \"localization\": {\n      \"description\": \"Settings for localization.\",\n      \"$ref\": \"#/components/schemas/Localization\"\n    },\n    \"nexo\": {\n      \"description\": \"Settings for a Terminal API integration.\",\n      \"$ref\": \"#/components/schemas/Nexo\"\n    },\n    \"offlineProcessing\": {\n      \"description\": \"Settings for [offline payment](https://docs.adyen.com/point-of-sale/offline-payments) features.\",\n      \"$ref\": \"#/components/schemas/OfflineProcessing\"\n    },\n    \"opi\": {\n      \"description\": \"Settings for an Oracle Payment Interface (OPI) integration.\",\n      \"$ref\": \"#/components/schemas/Opi\"\n    },\n    \"passcodes\": {\n      \"description\": \"Settings for [passcodes](https://docs.adyen.com/point-of-sale/managing-terminals/menu-access?tab=manage_passcodes_with_an_api_call_2#manage-passcodes)\
  \ features.\",\n      \"$ref\": \"#/components/schemas/Passcodes\"\n    },\n    \"payAtTable\": {\n      \"description\": \"Settings for [Pay-at-table](https://docs.adyen.com/point-of-sale/pay-at-x) features.\",\n      \"$ref\": \"#/components/schemas/PayAtTable\"\n    },\n    \"payment\": {\n      \"description\": \"Settings for payment features.\",\n      \"$ref\": \"#/components/schemas/Payment\"\n    },\n    \"receiptOptions\": {\n      \"description\": \"Generic receipt settings.\",\n      \"$ref\": \"#/components/schemas/ReceiptOptions\"\n    },\n    \"receiptPrinting\": {\n      \"description\": \"Transaction outcomes that you want the terminal to print a merchant receipt or a shopper receipt for.\",\n      \"$ref\": \"#/components/schemas/ReceiptPrinting\"\n    },\n    \"refunds\": {\n      \"description\": \"Settings for refunds.\",\n      \"$ref\": \"#/components/schemas/Refunds\"\n    },\n    \"signature\": {\n      \"description\": \"Settings to skip signature, sign on display,\
  \ or sign on receipt.\",\n      \"$ref\": \"#/components/schemas/Signature\"\n    },\n    \"standalone\": {\n      \"description\": \"Settings for [standalone](https://docs.adyen.com/point-of-sale/standalone/standalone-build/set-up-standalone#set-up-standalone-using-an-api-call) features.\",\n      \"$ref\": \"#/components/schemas/Standalone\"\n    },\n    \"surcharge\": {\n      \"description\": \"Settings for payment [surcharge](https://docs.adyen.com/point-of-sale/surcharge) features.\",\n      \"$ref\": \"#/components/schemas/Surcharge\"\n    },\n    \"tapToPay\": {\n      \"description\": \"Settings for Tap to Pay.\",\n      \"$ref\": \"#/components/schemas/TapToPay\"\n    },\n    \"timeouts\": {\n      \"description\": \"Settings for device [time-outs](https://docs.adyen.com/point-of-sale/pos-timeouts#device-time-out).\",\n      \"$ref\": \"#/components/schemas/Timeouts\"\n    },\n    \"wifiProfiles\": {\n      \"description\": \"Remote Wi-Fi profiles for WPA and WPA2 PSK and EAP\
  \ Wi-Fi networks.\",\n      \"$ref\": \"#/components/schemas/WifiProfiles\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-settings-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TerminalSettings
---
