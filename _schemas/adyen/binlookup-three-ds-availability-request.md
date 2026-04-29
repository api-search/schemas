---
description: ThreeDSAvailabilityRequest schema from Adyen API
layout: schema
name: ThreeDSAvailabilityRequest
properties_list:
- description: This field contains additional data, which may be required for a particular request. The `additionalData` object consists of entries, each of which includes the key and value.
  name: additionalData
  type: object
- description: List of brands.
  name: brands
  type: array
- description: Card number or BIN.
  name: cardNumber
  type: string
- description: The merchant account identifier.
  name: merchantAccount
  type: string
- description: A recurring detail reference corresponding to a card.
  name: recurringDetailReference
  type: string
- description: The shopper's reference to uniquely identify this shopper (e.g. user ID or account ID).
  name: shopperReference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/binlookup-three-ds-availability-request-schema.json
slug: binlookup-three-ds-availability-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/binlookup-three-ds-availability-request-schema.json\",\n  \"title\": \"ThreeDSAvailabilityRequest\",\n  \"description\": \"ThreeDSAvailabilityRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"additionalData\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"This field contains additional data, which may be required for a particular request.\\n\\nThe `additionalData` object consists of entries, each of which includes the key and value.\",\n      \"type\": \"object\"\n    },\n    \"brands\": {\n      \"description\": \"List of brands.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"cardNumber\": {\n      \"description\": \"Card number or BIN.\",\n      \"type\": \"string\"\
  \n    },\n    \"merchantAccount\": {\n      \"description\": \"The merchant account identifier.\",\n      \"type\": \"string\"\n    },\n    \"recurringDetailReference\": {\n      \"description\": \"A recurring detail reference corresponding to a card.\",\n      \"type\": \"string\"\n    },\n    \"shopperReference\": {\n      \"description\": \"The shopper's reference to uniquely identify this shopper (e.g. user ID or account ID).\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"merchantAccount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/binlookup-three-ds-availability-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ThreeDSAvailabilityRequest
---
