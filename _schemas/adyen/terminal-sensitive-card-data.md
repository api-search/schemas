---
description: This data structure could be CMS protected (EnvelopedData). In this case the data structure SensitiveCardData is replaced by the data structure ProtectedCardData of type ContentInformationType. When this data is protected, the exact content is unknown by the Sale System, and might include all the information which are required by an external backup POI Server to make a batch payment transaction in case of problem with the POI System. Sensitive information related to the payment card, entered or read by the Sale System.
layout: schema
name: SensitiveCardData
properties_list:
- description: ''
  name: PAN
  type: integer
- description: if EntryMode is File, Keyed or Manual.
  name: CardSeqNumb
  type: integer
- description: if EntryMode is File.
  name: ExpiryDate
  type: integer
- description: ''
  name: TrackData
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-sensitive-card-data-schema.json
slug: terminal-sensitive-card-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-sensitive-card-data-schema.json\",\n  \"title\": \"SensitiveCardData\",\n  \"description\": \"This data structure could be CMS protected (EnvelopedData). In this case the data structure SensitiveCardData is replaced by the data structure ProtectedCardData of type ContentInformationType. When this data is protected, the exact content is unknown by the Sale System, and might include all the information which are required by an external backup POI Server to make a batch payment transaction in case of problem with the POI System. Sensitive information related to the payment card, entered or read by the Sale System.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PAN\": {\n      \"type\": \"integer\",\n      \"minimum\": 8,\n      \"maximum\": 28\n    },\n    \"CardSeqNumb\": {\n      \"type\": \"integer\"\
  ,\n      \"minimum\": 2,\n      \"maximum\": 3,\n      \"description\": \"if EntryMode is File, Keyed or Manual.\"\n    },\n    \"ExpiryDate\": {\n      \"type\": \"integer\",\n      \"minimum\": 4,\n      \"maximum\": 4,\n      \"description\": \"if EntryMode is File.\"\n    },\n    \"TrackData\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TrackData\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-sensitive-card-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SensitiveCardData
---
