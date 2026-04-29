---
description: Service schema from AT&T API
layout: schema
name: Service
properties_list:
- description: Unique service identifier
  name: id
  type: string
- description: ''
  name: href
  type: string
- description: Service state
  name: state
  type: string
- description: Type of service
  name: serviceType
  type: string
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/mvnx-api-service-schema.json
slug: mvnx-api-service
source_filename: mvnx-api-service-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-service-schema.json\",\n  \"title\": \"Service\",\n  \"description\": \"Service schema from AT&T API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique service identifier\",\n      \"example\": \"svc-500123\"\n    },\n    \"href\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://devex-web.att.com/service/svc-500123\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Service state\",\n      \"enum\": [\n        \"active\",\n        \"inactive\",\n        \"reserved\"\n      ],\n      \"example\": \"active\"\n    },\n    \"serviceType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of service\",\n      \"example\": \"MOBILE\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-service-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: Service
---
