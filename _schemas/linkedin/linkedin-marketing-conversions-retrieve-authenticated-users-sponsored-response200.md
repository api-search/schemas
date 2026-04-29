---
description: RetrieveAuthenticatedUsersSponsoredResponse200 from LinkedIn API
layout: schema
name: RetrieveAuthenticatedUsersSponsoredResponse200
properties_list:
- description: ''
  name: paging
  type: object
- description: ''
  name: elements
  type: array
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-conversions-retrieve-authenticated-users-sponsored-response200-schema.json
slug: linkedin-marketing-conversions-retrieve-authenticated-users-sponsored-response200
source_filename: linkedin-marketing-conversions-retrieve-authenticated-users-sponsored-response200-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-conversions-retrieve-authenticated-users-sponsored-response200-schema.json\",\n  \"title\": \"RetrieveAuthenticatedUsersSponsoredResponse200\",\n  \"description\": \"RetrieveAuthenticatedUsersSponsoredResponse200 from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"paging\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"start\": {\n          \"type\": \"integer\"\n        },\n        \"count\": {\n          \"type\": \"integer\"\n        },\n        \"links\": {\n          \"type\": \"array\",\n          \"items\": {}\n        },\n        \"total\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"elements\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"\
  user\": {\n            \"type\": \"string\"\n          },\n          \"account\": {\n            \"type\": \"string\"\n          },\n          \"role\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-conversions-retrieve-authenticated-users-sponsored-response200-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: RetrieveAuthenticatedUsersSponsoredResponse200
---
