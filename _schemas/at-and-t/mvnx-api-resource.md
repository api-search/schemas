---
description: Resource schema from AT&T API
layout: schema
name: Resource
properties_list:
- description: Unique resource identifier
  name: id
  type: string
- description: Device or SIM name
  name: name
  type: string
- description: Type of resource
  name: resourceType
  type: string
- description: Resource operational status
  name: status
  type: string
- description: Device IMEI or SIM ICCID
  name: serialNumber
  type: string
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/mvnx-api-resource-schema.json
slug: mvnx-api-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-resource-schema.json\",\n  \"title\": \"Resource\",\n  \"description\": \"Resource schema from AT&T API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique resource identifier\",\n      \"example\": \"resource-500123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Device or SIM name\",\n      \"example\": \"Samsung Galaxy S25\"\n    },\n    \"resourceType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of resource\",\n      \"enum\": [\n        \"device\",\n        \"sim\"\n      ],\n      \"example\": \"device\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Resource operational status\",\n      \"enum\": [\n        \"active\",\n        \"inactive\"\
  ,\n        \"suspended\"\n      ],\n      \"example\": \"active\"\n    },\n    \"serialNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Device IMEI or SIM ICCID\",\n      \"example\": \"IMEI-123456789012345\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-resource-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: Resource
---
