---
description: A review of a place submitted by a user
layout: schema
name: Review
properties_list:
- description: The resource name of the review
  name: name
  type: string
- description: A human-readable relative time description
  name: relativePublishTimeDescription
  type: string
- description: The star rating of this review (1.0-5.0)
  name: rating
  type: number
- description: Timestamp of when the review was published
  name: publishTime
  type: string
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-places-review-schema.json
slug: google-maps-places-review
source_filename: google-maps-places-review-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Review\",\n  \"type\": \"object\",\n  \"description\": \"A review of a place submitted by a user\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the review\"\n    },\n    \"relativePublishTimeDescription\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable relative time description\"\n    },\n    \"rating\": {\n      \"type\": \"number\",\n      \"description\": \"The star rating of this review (1.0-5.0)\"\n    },\n    \"publishTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of when the review was published\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-places-review-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: Review
---
