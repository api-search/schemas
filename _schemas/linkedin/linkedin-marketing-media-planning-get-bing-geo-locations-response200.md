---
description: GetBingGeoLocationsResponse200 from LinkedIn API
layout: schema
name: GetBingGeoLocationsResponse200
properties_list:
- description: ''
  name: paging
  type: object
- description: ''
  name: elements
  type: array
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-media-planning-get-bing-geo-locations-response200-schema.json
slug: linkedin-marketing-media-planning-get-bing-geo-locations-response200
source_filename: linkedin-marketing-media-planning-get-bing-geo-locations-response200-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-media-planning-get-bing-geo-locations-response200-schema.json\",\n  \"title\": \"GetBingGeoLocationsResponse200\",\n  \"description\": \"GetBingGeoLocationsResponse200 from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"paging\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"start\": {\n          \"type\": \"integer\"\n        },\n        \"count\": {\n          \"type\": \"integer\"\n        },\n        \"links\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\"\n              },\n              \"rel\": {\n                \"type\": \"string\"\n              },\n              \"href\": {\n                \"type\"\
  : \"string\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"elements\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"urn\": {\n            \"type\": \"string\"\n          },\n          \"facetUrn\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-media-planning-get-bing-geo-locations-response200-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: GetBingGeoLocationsResponse200
---
