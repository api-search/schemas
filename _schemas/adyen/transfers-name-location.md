---
description: NameLocation schema from Adyen API
layout: schema
name: NameLocation
properties_list:
- description: The city where the merchant is located.
  name: city
  type: string
- description: The country where the merchant is located in [three-letter country code](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-3) format.
  name: country
  type: string
- description: The home country in [three-digit country code](https://en.wikipedia.org/wiki/ISO_3166-1_numeric) format, used for government-controlled merchants such as embassies.
  name: countryOfOrigin
  type: string
- description: The name of the merchant's shop or service.
  name: name
  type: string
- description: The raw data.
  name: rawData
  type: string
- description: The state where the merchant is located.
  name: state
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfers-name-location-schema.json
slug: transfers-name-location
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-name-location-schema.json\",\n  \"title\": \"NameLocation\",\n  \"description\": \"NameLocation schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"city\": {\n      \"description\": \"The city where the merchant is located.\",\n      \"type\": \"string\"\n    },\n    \"country\": {\n      \"description\": \"The country where the merchant is located in [three-letter country code](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-3) format.\",\n      \"type\": \"string\"\n    },\n    \"countryOfOrigin\": {\n      \"description\": \"The home country in [three-digit country code](https://en.wikipedia.org/wiki/ISO_3166-1_numeric) format, used for government-controlled merchants such as embassies.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The name\
  \ of the merchant's shop or service.\",\n      \"type\": \"string\"\n    },\n    \"rawData\": {\n      \"description\": \"The raw data.\",\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"description\": \"The state where the merchant is located.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-name-location-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: NameLocation
---
