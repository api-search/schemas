---
description: Organization profile data
layout: schema
name: OrganizationResponse
properties_list:
- description: Organization ID
  name: id
  type: integer
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: tagline
  type: object
- description: ''
  name: localizedName
  type: string
- description: ''
  name: localizedDescription
  type: string
- description: ''
  name: localizedTagline
  type: string
- description: ''
  name: vanityName
  type: string
- description: ''
  name: organizationType
  type: string
- description: ''
  name: staffCountRange
  type: string
- description: ''
  name: industriesV2
  type: array
- description: ''
  name: logoV2
  type: object
- description: ''
  name: coverPhotoV2
  type: object
- description: ''
  name: locations
  type: array
- description: ''
  name: foundedOn
  type: object
- description: ''
  name: entityStatus
  type: string
- description: ''
  name: created
  type: object
- description: ''
  name: lastModified
  type: object
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-regulations-data-portability-organization-response-schema.json
slug: linkedin-regulations-data-portability-organization-response
source_filename: linkedin-regulations-data-portability-organization-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-regulations-data-portability-organization-response-schema.json\",\n  \"title\": \"OrganizationResponse\",\n  \"description\": \"Organization profile data\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Organization ID\",\n      \"example\": 10002687\n    },\n    \"name\": {\n      \"$ref\": \"#/components/schemas/LocalizedString\"\n    },\n    \"description\": {\n      \"$ref\": \"#/components/schemas/LocalizedString\"\n    },\n    \"tagline\": {\n      \"$ref\": \"#/components/schemas/LocalizedString\"\n    },\n    \"localizedName\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"localizedDescription\": {\n      \"type\": \"string\",\n      \"example\": \"Leading\
  \ provider of innovative solutions\"\n    },\n    \"localizedTagline\": {\n      \"type\": \"string\",\n      \"example\": \"Innovation at its best\"\n    },\n    \"vanityName\": {\n      \"type\": \"string\",\n      \"example\": \"acme-corp\"\n    },\n    \"organizationType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PUBLIC_COMPANY\",\n        \"PRIVATELY_HELD\",\n        \"GOVERNMENT_AGENCY\",\n        \"NON_PROFIT\",\n        \"PARTNERSHIP\"\n      ],\n      \"example\": \"PRIVATELY_HELD\"\n    },\n    \"staffCountRange\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SIZE_1\",\n        \"SIZE_2_TO_10\",\n        \"SIZE_11_TO_50\",\n        \"SIZE_51_TO_200\",\n        \"SIZE_201_TO_500\",\n        \"SIZE_501_TO_1000\",\n        \"SIZE_1001_TO_5000\",\n        \"SIZE_5001_TO_10000\",\n        \"SIZE_10001_OR_MORE\"\n      ],\n      \"example\": \"SIZE_201_TO_500\"\n    },\n    \"industriesV2\": {\n      \"type\": \"array\",\n      \"items\": {\n  \
  \      \"type\": \"string\"\n      },\n      \"example\": [\n        \"urn:li:industry:33\"\n      ]\n    },\n    \"logoV2\": {\n      \"$ref\": \"#/components/schemas/ImageReference\"\n    },\n    \"coverPhotoV2\": {\n      \"$ref\": \"#/components/schemas/ImageReference\"\n    },\n    \"locations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/OrganizationLocation\"\n      }\n    },\n    \"foundedOn\": {\n      \"$ref\": \"#/components/schemas/DateInfo\"\n    },\n    \"entityStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"INACTIVE\"\n      ],\n      \"example\": \"ACTIVE\"\n    },\n    \"created\": {\n      \"$ref\": \"#/components/schemas/Timestamp\"\n    },\n    \"lastModified\": {\n      \"$ref\": \"#/components/schemas/Timestamp\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-regulations-data-portability-organization-response-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: OrganizationResponse
---
