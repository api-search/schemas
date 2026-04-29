---
description: ''
layout: schema
name: ListingCreate
properties_list:
- description: The display name of the listing.
  name: name
  type: string
- description: The full description of the property.
  name: description
  type: string
- description: The type of property being listed.
  name: property_type
  type: string
- description: The type of room or space being offered.
  name: room_type
  type: string
- description: ''
  name: address
  type: object
- description: The number of bedrooms in the property.
  name: bedrooms
  type: integer
- description: The number of bathrooms in the property.
  name: bathrooms
  type: number
- description: The total number of beds in the property.
  name: beds
  type: integer
- description: The maximum number of guests allowed.
  name: max_guests
  type: integer
- description: The list of amenity identifiers available at the property.
  name: amenities
  type: array
- description: The house rules and guidelines for guests.
  name: house_rules
  type: string
- description: The earliest check-in time in HH:MM format.
  name: check_in_time
  type: string
- description: The latest check-out time in HH:MM format.
  name: check_out_time
  type: string
- description: The cancellation policy applied to the listing.
  name: cancellation_policy
  type: string
provider_name: airbnb
provider_slug: airbnb
schema_file: json-schema/airbnb-listing-create-schema.json
slug: airbnb-listing-create
source_filename: airbnb-listing-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-listing-create-schema.json\",\n  \"title\": \"ListingCreate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the listing.\",\n      \"maxLength\": 50\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The full description of the property.\",\n      \"maxLength\": 5000\n    },\n    \"property_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of property being listed.\",\n      \"enum\": [\n        \"apartment\",\n        \"house\",\n        \"secondary_unit\",\n        \"unique_space\",\n        \"bed_and_breakfast\",\n        \"boutique_hotel\"\n      ]\n    },\n    \"room_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of room or\
  \ space being offered.\",\n      \"enum\": [\n        \"entire_home\",\n        \"private_room\",\n        \"shared_room\"\n      ]\n    },\n    \"address\": {\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"bedrooms\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of bedrooms in the property.\",\n      \"minimum\": 0\n    },\n    \"bathrooms\": {\n      \"type\": \"number\",\n      \"description\": \"The number of bathrooms in the property.\",\n      \"minimum\": 0\n    },\n    \"beds\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of beds in the property.\",\n      \"minimum\": 0\n    },\n    \"max_guests\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of guests allowed.\",\n      \"minimum\": 1\n    },\n    \"amenities\": {\n      \"type\": \"array\",\n      \"description\": \"The list of amenity identifiers available at the property.\",\n      \"items\": {\n        \"type\": \"string\"\
  \n      }\n    },\n    \"house_rules\": {\n      \"type\": \"string\",\n      \"description\": \"The house rules and guidelines for guests.\"\n    },\n    \"check_in_time\": {\n      \"type\": \"string\",\n      \"description\": \"The earliest check-in time in HH:MM format.\",\n      \"pattern\": \"^[0-2][0-9]:[0-5][0-9]$\"\n    },\n    \"check_out_time\": {\n      \"type\": \"string\",\n      \"description\": \"The latest check-out time in HH:MM format.\",\n      \"pattern\": \"^[0-2][0-9]:[0-5][0-9]$\"\n    },\n    \"cancellation_policy\": {\n      \"type\": \"string\",\n      \"description\": \"The cancellation policy applied to the listing.\",\n      \"enum\": [\n        \"flexible\",\n        \"moderate\",\n        \"strict\",\n        \"strict_14_with_grace_period\",\n        \"super_strict_30\",\n        \"super_strict_60\"\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"property_type\",\n    \"room_type\",\n    \"address\",\n    \"max_guests\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-listing-create-schema.json
tags: []
title: ListingCreate
---
