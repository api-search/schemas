---
description: Request to check AT&T wireline service availability at a location
layout: schema
name: Service Qualification Request
properties_list:
- description: ''
  name: address
  type: object
provider_name: AT&T
provider_slug: atandt
schema_file: json-schema/enterprise-apis-service-qualification-request-schema.json
slug: enterprise-apis-service-qualification-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://devex-web.att.com/schemas/enterprise/service-qualification-request\",\n  \"title\": \"Service Qualification Request\",\n  \"description\": \"Request to check AT&T wireline service availability at a location\",\n  \"type\": \"object\",\n  \"required\": [\n    \"address\"\n  ],\n  \"properties\": {\n    \"address\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"streetAddress\",\n        \"city\",\n        \"state\",\n        \"postalCode\",\n        \"country\"\n      ],\n      \"properties\": {\n        \"streetAddress\": {\n          \"type\": \"string\"\n        },\n        \"city\": {\n          \"type\": \"string\"\n        },\n        \"state\": {\n          \"type\": \"string\"\n        },\n        \"postalCode\": {\n          \"type\": \"string\"\n        },\n        \"country\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/json-schema/enterprise-apis-service-qualification-request-schema.json
tags:
- Telecommunications
- Fortune 100
- Wireless
- Wireline
- Broadband
- Enterprise
- 5G
- Network
title: Service Qualification Request
---
