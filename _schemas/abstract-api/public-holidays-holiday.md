---
description: A public holiday entry
layout: schema
name: Holiday
properties_list:
- description: Holiday name in English
  name: name
  type: string
- description: Holiday name in local language
  name: name_local
  type: string
- description: Language of the local name
  name: language
  type: string
- description: Additional details about the holiday
  name: description
  type: string
- description: Country code
  name: country
  type: string
- description: Specific region where holiday applies
  name: location
  type: string
- description: Holiday classification
  name: type
  type: string
- description: Holiday date in MM/DD/YYYY format
  name: date
  type: string
- description: Year of the holiday
  name: date_year
  type: string
- description: Month of the holiday
  name: date_month
  type: string
- description: Day of the holiday
  name: date_day
  type: string
- description: Day of the week
  name: week_day
  type: string
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/public-holidays-holiday-schema.json
slug: public-holidays-holiday
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/public-holidays-holiday-schema.json\",\n  \"title\": \"Holiday\",\n  \"description\": \"A public holiday entry\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Holiday name in English\",\n      \"example\": \"Easter Sunday\"\n    },\n    \"name_local\": {\n      \"type\": \"string\",\n      \"description\": \"Holiday name in local language\",\n      \"example\": \"Paques\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"Language of the local name\",\n      \"example\": \"FR\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Additional details about the holiday\",\n      \"example\": \"Easter Sunday marks the resurrection of Jesus Christ\"\n    },\n    \"country\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Country code\",\n      \"example\": \"US\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"Specific region where holiday applies\",\n      \"example\": \"\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Holiday classification\",\n      \"example\": \"National\",\n      \"enum\": [\n        \"National\",\n        \"Local\",\n        \"Religious\",\n        \"Observance\",\n        \"Season\",\n        \"Clock Change/Daylight Saving Time\"\n      ]\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"Holiday date in MM/DD/YYYY format\",\n      \"example\": \"04/20/2025\"\n    },\n    \"date_year\": {\n      \"type\": \"string\",\n      \"description\": \"Year of the holiday\",\n      \"example\": \"2025\"\n    },\n    \"date_month\": {\n      \"type\": \"string\",\n      \"description\": \"Month of the holiday\",\n      \"example\": \"\
  04\"\n    },\n    \"date_day\": {\n      \"type\": \"string\",\n      \"description\": \"Day of the holiday\",\n      \"example\": \"20\"\n    },\n    \"week_day\": {\n      \"type\": \"string\",\n      \"description\": \"Day of the week\",\n      \"example\": \"Sunday\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/public-holidays-holiday-schema.json
tags:
- Avatars
- Company Enrichment
- Contacts
- Currencies
- Email Validation
- Exchange Rates
- IBAN Validation
- Image Processing
- IP Geolocation
- IP Intelligence
- Phone Validation
- Public Holidays
- Screenshots
- Timezones
- VAT Validation
- Web Scraping
title: Holiday
---
