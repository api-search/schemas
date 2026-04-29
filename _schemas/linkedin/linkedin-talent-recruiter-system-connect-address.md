---
description: Address from LinkedIn API
layout: schema
name: Address
properties_list:
- description: ''
  name: line1
  type: string
- description: ''
  name: city
  type: string
- description: ''
  name: geographicArea
  type: string
- description: ''
  name: geographicAreaType
  type: string
- description: ''
  name: postalCode
  type: string
- description: ''
  name: country
  type: string
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-talent-recruiter-system-connect-address-schema.json
slug: linkedin-talent-recruiter-system-connect-address
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-recruiter-system-connect-address-schema.json\",\n  \"title\": \"Address\",\n  \"description\": \"Address from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"line1\": {\n      \"type\": \"string\",\n      \"example\": \"123 Main Street\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"example\": \"San Francisco\"\n    },\n    \"geographicArea\": {\n      \"type\": \"string\",\n      \"example\": \"CA\"\n    },\n    \"geographicAreaType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"STATE\",\n        \"PROVINCE\"\n      ],\n      \"example\": \"STATE\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"example\": \"94102\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"example\": \"US\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-recruiter-system-connect-address-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: Address
---
