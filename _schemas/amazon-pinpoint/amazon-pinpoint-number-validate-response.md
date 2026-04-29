---
description: Provides information about a phone number.
layout: schema
name: NumberValidateResponse
properties_list:
- description: ''
  name: Carrier
  type: object
- description: ''
  name: City
  type: object
- description: ''
  name: CleansedPhoneNumberE164
  type: object
- description: ''
  name: CleansedPhoneNumberNational
  type: object
- description: ''
  name: Country
  type: object
- description: ''
  name: CountryCodeIso2
  type: object
- description: ''
  name: CountryCodeNumeric
  type: object
- description: ''
  name: County
  type: object
- description: ''
  name: OriginalCountryCodeIso2
  type: object
- description: ''
  name: OriginalPhoneNumber
  type: object
- description: ''
  name: PhoneType
  type: object
- description: ''
  name: PhoneTypeCode
  type: object
- description: ''
  name: Timezone
  type: object
- description: ''
  name: ZipCode
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-number-validate-response-schema.json
slug: amazon-pinpoint-number-validate-response
source_filename: amazon-pinpoint-number-validate-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-number-validate-response-schema.json\",\n  \"title\": \"NumberValidateResponse\",\n  \"description\": \"Provides information about a phone number.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Carrier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The carrier or service provider that the phone number is currently registered with. In some countries and regions, this value may be the carrier or service provider that the phone number was originally registered with.\"\n        }\n      ]\n    },\n    \"City\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the city where the phone\
  \ number was originally registered.\"\n        }\n      ]\n    },\n    \"CleansedPhoneNumberE164\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The cleansed phone number, in E.164 format, for the location where the phone number was originally registered.\"\n        }\n      ]\n    },\n    \"CleansedPhoneNumberNational\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The cleansed phone number, in the format for the location where the phone number was originally registered.\"\n        }\n      ]\n    },\n    \"Country\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the country or region where the phone number was originally registered.\"\n        }\n      ]\n    },\n    \"CountryCodeIso2\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The two-character code, in ISO 3166-1 alpha-2 format, for the country or region where the phone number was originally registered.\"\n        }\n      ]\n    },\n    \"CountryCodeNumeric\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The numeric code for the country or region where the phone number was originally registered.\"\n        }\n      ]\n    },\n    \"County\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the county where the phone number was originally registered.\"\n        }\n      ]\n    },\n    \"OriginalCountryCodeIso2\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n\
  \          \"description\": \"The two-character code, in ISO 3166-1 alpha-2 format, that was sent in the request body.\"\n        }\n      ]\n    },\n    \"OriginalPhoneNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The phone number that was sent in the request body.\"\n        }\n      ]\n    },\n    \"PhoneType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The description of the phone type. Valid values are: MOBILE, LANDLINE, VOIP,\\n                  INVALID, PREPAID, and OTHER.\"\n        }\n      ]\n    },\n    \"PhoneTypeCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The phone type, represented by an integer. Valid values are: 0 (mobile), 1 (landline), 2 (VoIP), 3 (invalid), 4 (other),\
  \ and 5 (prepaid).\"\n        }\n      ]\n    },\n    \"Timezone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The time zone for the location where the phone number was originally registered.\"\n        }\n      ]\n    },\n    \"ZipCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The postal or ZIP code for the location where the phone number was originally registered.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-number-validate-response-schema.json
tags:
- AWS
- Campaigns
- Communications
- Email
- Marketing
- Messaging
- Push Notifications
- SMS
- Voice
- Customer Engagement
- Segmentation
- Journeys
- Analytics
title: NumberValidateResponse
---
