---
description: emergency contact number
layout: schema
name: EmergencyContact
properties_list:
- description: Adressee name (e.g. in case of emergency purpose it corresponds to name of the person to be contacted).
  name: addresseeName
  type: string
- description: Country code of the country (ISO3166-1). E.g. "US" for the United States
  name: countryCode
  type: string
- description: Phone number. Composed of digits only. The number of digits depends on the country.
  name: number
  type: string
- description: additional details
  name: text
  type: string
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/seat-map-display-emergency-contact-schema.json
slug: seat-map-display-emergency-contact
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-emergency-contact-schema.json\",\n  \"title\": \"EmergencyContact\",\n  \"description\": \"emergency contact number\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"addresseeName\": {\n      \"type\": \"string\",\n      \"description\": \"Adressee name (e.g. in case of emergency purpose it corresponds to name of the person to be contacted).\",\n      \"pattern\": \"[a-zA-Z -]\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"Country code of the country (ISO3166-1). E.g. \\\"US\\\" for the United States\",\n      \"pattern\": \"[A-Z]{2}\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number. Composed of digits only. The number of digits depends on the country.\",\n      \"pattern\": \"[0-9]{1,15}\"\
  \n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"additional details\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-emergency-contact-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: EmergencyContact
---
