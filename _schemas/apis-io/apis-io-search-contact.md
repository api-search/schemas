---
description: Information on contacting the API support
layout: schema
name: Contact
properties_list:
- description: ''
  name: FN
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: organizationName
  type: string
- description: ''
  name: adr
  type: string
- description: ''
  name: tel
  type: string
- description: ''
  name: X-github
  type: string
- description: ''
  name: photo
  type: string
- description: ''
  name: vCard
  type: string
- description: ''
  name: url
  type: string
provider_name: APIs.io
provider_slug: apis-io
schema_file: json-schema/apis-io-search-contact-schema.json
slug: apis-io-search-contact
source_filename: apis-io-search-contact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/json-schema/apis-io-search-contact-schema.json\",\n  \"title\": \"Contact\",\n  \"description\": \"Information on contacting the API support\",\n  \"required\": [\n    \"FN\"\n  ],\n  \"properties\": {\n    \"FN\": {\n      \"type\": \"string\",\n      \"minLength\": 1\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\"\n    },\n    \"organizationName\": {\n      \"type\": \"string\",\n      \"minLength\": 1\n    },\n    \"adr\": {\n      \"type\": \"string\"\n    },\n    \"tel\": {\n      \"type\": \"string\",\n      \"minLength\": 1\n    },\n    \"X-github\": {\n      \"type\": \"string\"\n    },\n    \"photo\": {\n      \"type\": \"string\",\n      \"pattern\": \"^(http)|(https)://(.*)$\"\n    },\n    \"vCard\": {\n      \"type\": \"string\",\n      \"pattern\": \"^(http)|(https)://(.*)$\"\
  \n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"pattern\": \"^(http)|(https)://(.*)$\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/json-schema/apis-io-search-contact-schema.json
tags:
- API Aggregation
- API Directory
- API Discovery
- API Indexing
- API Rating
- API Search
- APIs.json
- Search Engine
title: Contact
---
