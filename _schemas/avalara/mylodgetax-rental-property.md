---
description: RentalProperty schema from Avalara API
layout: schema
name: RentalProperty
properties_list:
- description: ''
  name: propertyId
  type: string
- description: ''
  name: propertyName
  type: string
- description: ''
  name: address
  type: object
- description: Platforms where the property is listed (e.g., Airbnb, VRBO)
  name: listingPlatforms
  type: array
- description: ''
  name: propertyType
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/mylodgetax-rental-property-schema.json
slug: mylodgetax-rental-property
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/mylodgetax-rental-property-schema.json\",\n  \"title\": \"RentalProperty\",\n  \"description\": \"RentalProperty schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"propertyId\": {\n      \"type\": \"string\"\n    },\n    \"propertyName\": {\n      \"type\": \"string\"\n    },\n    \"address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"line1\": {\n          \"type\": \"string\"\n        },\n        \"city\": {\n          \"type\": \"string\"\n        },\n        \"region\": {\n          \"type\": \"string\"\n        },\n        \"postalCode\": {\n          \"type\": \"string\"\n        },\n        \"country\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"listingPlatforms\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"\
  type\": \"string\"\n      },\n      \"description\": \"Platforms where the property is listed (e.g., Airbnb, VRBO)\"\n    },\n    \"propertyType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"House\",\n        \"Apartment\",\n        \"Condo\",\n        \"Room\",\n        \"Other\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/mylodgetax-rental-property-schema.json
tags:
- Taxes
title: RentalProperty
---
