---
description: ListUploadRequest from LinkedIn API
layout: schema
name: ListUploadRequest
properties_list:
- description: Media URN of the uploaded file
  name: inputFile
  type: string
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-audience-list-upload-request-schema.json
slug: linkedin-marketing-audience-list-upload-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-list-upload-request-schema.json\",\n  \"title\": \"ListUploadRequest\",\n  \"description\": \"ListUploadRequest from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputFile\": {\n      \"type\": \"string\",\n      \"description\": \"Media URN of the uploaded file\",\n      \"example\": \"urn:li:digitalmediaAsset:C5605AQH2...\"\n    }\n  },\n  \"required\": [\n    \"inputFile\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-list-upload-request-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: ListUploadRequest
---
