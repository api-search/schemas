---
description: phone information
layout: schema
name: Phone
properties_list:
- description: Category of the contact element
  name: category
  type: string
- description: Adressee name (e.g. in case of emergency purpose it corresponds to name of the person to be contacted).
  name: addresseeName
  type: string
- description: ''
  name: deviceType
  type: object
- description: Country code of the country (ISO3166-1). E.g. "US" for the United States
  name: countryCode
  type: string
- description: Country calling code of the phone number, as defined by the International Communication Union. Examples - "1" for US, "371" for Latvia.
  name: countryCallingCode
  type: string
- description: Corresponds to a regional code or a city code. The length of the field varies depending on the area.
  name: areaCode
  type: string
- description: Phone number. Composed of digits only. The number of digits depends on the country.
  name: number
  type: string
- description: Extension of the phone
  name: extension
  type: string
- description: String containing the full phone number - applicable only when a structured phone (i.e. countryCallingCode + number) is not provided
  name: text
  type: string
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/seat-map-display-phone-schema.json
slug: seat-map-display-phone
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-phone-schema.json\",\n  \"title\": \"Phone\",\n  \"description\": \"phone information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"category\": {\n      \"description\": \"Category of the contact element\",\n      \"type\": \"string\",\n      \"enum\": [\n        \"BUSINESS\",\n        \"PERSONAL\",\n        \"OTHER\"\n      ]\n    },\n    \"addresseeName\": {\n      \"type\": \"string\",\n      \"description\": \"Adressee name (e.g. in case of emergency purpose it corresponds to name of the person to be contacted).\",\n      \"pattern\": \"[a-zA-Z -]\"\n    },\n    \"deviceType\": {\n      \"$ref\": \"#/definitions/PhoneDeviceType\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"Country code of the country (ISO3166-1). E.g. \\\"US\\\"\
  \ for the United States\",\n      \"pattern\": \"[A-Z]{2}\"\n    },\n    \"countryCallingCode\": {\n      \"type\": \"string\",\n      \"description\": \"Country calling code of the phone number, as defined by the International Communication Union. Examples - \\\"1\\\" for US, \\\"371\\\" for Latvia.\",\n      \"pattern\": \"[0-9+]{2,5}\"\n    },\n    \"areaCode\": {\n      \"type\": \"string\",\n      \"description\": \"Corresponds to a regional code or a city code. The length of the field varies depending on the area.\",\n      \"pattern\": \"[0-9]{1,4}\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number. Composed of digits only. The number of digits depends on the country.\",\n      \"pattern\": \"[0-9]{1,15}\"\n    },\n    \"extension\": {\n      \"type\": \"string\",\n      \"description\": \"Extension of the phone\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"String containing the full phone number -\
  \ applicable only when a structured phone (i.e. countryCallingCode + number) is not provided\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-phone-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: Phone
---
