---
description: A place object returned by the Google Places API.
layout: schema
name: Google Place
properties_list:
- description: Resource name of the place.
  name: name
  type: string
- description: The unique identifier of a place.
  name: id
  type: string
- description: The localized name of the place.
  name: displayName
  type: object
- description: A set of type tags for this place.
  name: types
  type: array
- description: A human-readable address for this place.
  name: formattedAddress
  type: string
- description: The position of this place.
  name: location
  type: object
- description: The average user rating for this place.
  name: rating
  type: number
- description: The total number of user ratings.
  name: userRatingCount
  type: integer
- description: The authoritative website for this place.
  name: websiteUri
  type: string
- description: The regular opening hours.
  name: regularOpeningHours
  type: object
- description: Photos of this place.
  name: photos
  type: array
- description: Reviews of this place.
  name: reviews
  type: array
provider_name: Google Places
provider_slug: google-places
schema_file: json-schema/Place.json
slug: Place
source_filename: Place.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"Place.json\",\n  \"title\": \"Google Place\",\n  \"description\": \"A place object returned by the Google Places API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Resource name of the place.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of a place.\"\n    },\n    \"displayName\": {\n      \"type\": \"object\",\n      \"description\": \"The localized name of the place.\",\n      \"properties\": {\n        \"text\": {\n          \"type\": \"string\"\n        },\n        \"languageCode\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"types\": {\n      \"type\": \"array\",\n      \"description\": \"A set of type tags for this place.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"formattedAddress\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"A human-readable address for this place.\"\n    },\n    \"location\": {\n      \"type\": \"object\",\n      \"description\": \"The position of this place.\",\n      \"properties\": {\n        \"latitude\": {\n          \"type\": \"number\"\n        },\n        \"longitude\": {\n          \"type\": \"number\"\n        }\n      }\n    },\n    \"rating\": {\n      \"type\": \"number\",\n      \"description\": \"The average user rating for this place.\"\n    },\n    \"userRatingCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of user ratings.\"\n    },\n    \"websiteUri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The authoritative website for this place.\"\n    },\n    \"regularOpeningHours\": {\n      \"type\": \"object\",\n      \"description\": \"The regular opening hours.\",\n      \"properties\": {\n        \"openNow\": {\n          \"type\": \"boolean\"\n        },\n\
  \        \"periods\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\"\n          }\n        }\n      }\n    },\n    \"photos\": {\n      \"type\": \"array\",\n      \"description\": \"Photos of this place.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"widthPx\": {\n            \"type\": \"integer\"\n          },\n          \"heightPx\": {\n            \"type\": \"integer\"\n          }\n        }\n      }\n    },\n    \"reviews\": {\n      \"type\": \"array\",\n      \"description\": \"Reviews of this place.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"rating\": {\n            \"type\": \"number\"\n          },\n          \"text\": {\n            \"type\": \"object\",\n            \"properties\": {\n       \
  \       \"text\": {\n                \"type\": \"string\"\n              },\n              \"languageCode\": {\n                \"type\": \"string\"\n              }\n            }\n          },\n          \"publishTime\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-places/refs/heads/main/json-schema/Place.json
tags:
- Geolocation
- Google
- Locations
- Maps
- Places
- Points of Interest
title: Google Place
---
