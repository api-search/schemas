---
description: Request to port phone numbers from another carrier
layout: schema
name: PortInRequest
properties_list:
- description: The site to assign ported numbers to
  name: siteId
  type: string
- description: The SIP peer to assign ported numbers to
  name: peerId
  type: string
- description: The billing telephone number for the account being ported
  name: billingTelephoneNumber
  type: string
- description: ''
  name: subscriber
  type: object
- description: The name of the current carrier
  name: losingCarrierName
  type: string
- description: List of phone numbers to port
  name: listOfPhoneNumbers
  type: array
- description: Requested Firm Order Commitment date
  name: requestedFocDate
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/phone-numbers-port-in-request-schema.json
slug: phone-numbers-port-in-request
source_filename: phone-numbers-port-in-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-port-in-request-schema.json\",\n  \"title\": \"PortInRequest\",\n  \"description\": \"Request to port phone numbers from another carrier\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"siteId\": {\n      \"type\": \"string\",\n      \"description\": \"The site to assign ported numbers to\"\n    },\n    \"peerId\": {\n      \"type\": \"string\",\n      \"description\": \"The SIP peer to assign ported numbers to\"\n    },\n    \"billingTelephoneNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The billing telephone number for the account being ported\"\n    },\n    \"subscriber\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"subscriberType\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"BUSINESS\",\n            \"RESIDENTIAL\"\
  \n          ],\n          \"description\": \"The type of subscriber\"\n        },\n        \"businessName\": {\n          \"type\": \"string\",\n          \"description\": \"The business name (for business subscribers)\"\n        },\n        \"firstName\": {\n          \"type\": \"string\",\n          \"description\": \"The subscriber first name\"\n        },\n        \"lastName\": {\n          \"type\": \"string\",\n          \"description\": \"The subscriber last name\"\n        },\n        \"serviceAddress\": {\n          \"$ref\": \"#/components/schemas/Address\"\n        }\n      }\n    },\n    \"losingCarrierName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the current carrier\"\n    },\n    \"listOfPhoneNumbers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of phone numbers to port\"\n    },\n    \"requestedFocDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\
  ,\n      \"description\": \"Requested Firm Order Commitment date\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-port-in-request-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: PortInRequest
---
