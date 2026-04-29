---
description: ''
layout: schema
name: Phone
properties_list:
- description: 'The match status between either of the input names (person or business) and the queried entity. Possible values are: * not-found * match * no-match'
  name: matchToName
  type: string
- description: The line type of the phone number. * landline - Traditional wired phone line. * fixed-voip - VOIP-based fixed line phones. * mobile - Wireless phone line. * voicemail - Voicemail-only service. * toll-
  name: lineType
  type: string
- description: True if the phone number is valid.
  name: valid
  type: boolean
- description: The company that provides voice and/or data services for the phone number. Carriers are returned at the MVNO level.
  name: phoneNumberCarrier
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-identity-insights-for-transactions-phone-schema.json
slug: mastercard-identity-insights-for-transactions-phone
source_filename: mastercard-identity-insights-for-transactions-phone-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Phone\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"matchToName\": {\n      \"type\": \"string\",\n      \"description\": \"The match status between either of the input names (person or business) and the queried entity. Possible values are: * not-found * match * no-match\"\n    },\n    \"lineType\": {\n      \"type\": \"string\",\n      \"description\": \"The line type of the phone number. * landline - Traditional wired phone line. * fixed-voip - VOIP-based fixed line phones. * mobile - Wireless phone line. * voicemail - Voicemail-only service. * toll-free - Callee pays for call. * premium - Caller pays a premium for the call-e.g. 976 area code. * non-fixed-voip - Skype, for example. * other - Anything that does not match the previous categories.\"\n    },\n    \"valid\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the phone number is valid.\"\n    },\n    \"\
  phoneNumberCarrier\": {\n      \"type\": \"string\",\n      \"description\": \"The company that provides voice and/or data services for the phone number. Carriers are returned at the MVNO level.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-identity-insights-for-transactions-phone-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Phone
---
