---
description: OrganizationLocation from LinkedIn API
layout: schema
name: OrganizationLocation
properties_list:
- description: ''
  name: locationType
  type: string
- description: ''
  name: address
  type: object
- description: ''
  name: geoLocation
  type: string
- description: ''
  name: staffCountRange
  type: string
- description: ''
  name: description
  type: object
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-regulations-data-portability-organization-location-schema.json
slug: linkedin-regulations-data-portability-organization-location
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-regulations-data-portability-organization-location-schema.json\",\n  \"title\": \"OrganizationLocation\",\n  \"description\": \"OrganizationLocation from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"locationType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"HEADQUARTERS\",\n        \"OTHER\"\n      ],\n      \"example\": \"HEADQUARTERS\"\n    },\n    \"address\": {\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"geoLocation\": {\n      \"type\": \"string\",\n      \"example\": \"urn:li:geo:101308755\"\n    },\n    \"staffCountRange\": {\n      \"type\": \"string\",\n      \"example\": \"SIZE_1\"\n    },\n    \"description\": {\n      \"$ref\": \"#/components/schemas/LocalizedString\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-regulations-data-portability-organization-location-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: OrganizationLocation
---
