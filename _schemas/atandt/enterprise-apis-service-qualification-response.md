---
description: Results of AT&T wireline service qualification check
layout: schema
name: Service Qualification Response
properties_list:
- description: ''
  name: qualificationId
  type: string
- description: ''
  name: qualificationDate
  type: string
- description: ''
  name: serviceQualificationItems
  type: array
provider_name: AT&T
provider_slug: atandt
schema_file: json-schema/enterprise-apis-service-qualification-response-schema.json
slug: enterprise-apis-service-qualification-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://devex-web.att.com/schemas/enterprise/service-qualification-response\",\n  \"title\": \"Service Qualification Response\",\n  \"description\": \"Results of AT&T wireline service qualification check\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"qualificationId\": {\n      \"type\": \"string\"\n    },\n    \"qualificationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"serviceQualificationItems\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"state\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"done\",\n              \"terminatedWithError\"\n            ]\n          },\n          \"serviceSpecification\": {\n            \"type\": \"object\",\n            \"properties\": {\n\
  \              \"name\": {\n                \"type\": \"string\"\n              }\n            }\n          },\n          \"eligibilityUnavailabilityReason\": {\n            \"type\": [\n              \"string\",\n              \"null\"\n            ]\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/json-schema/enterprise-apis-service-qualification-response-schema.json
tags:
- Telecommunications
- Fortune 100
- Wireless
- Wireline
- Broadband
- Enterprise
- 5G
- Network
title: Service Qualification Response
---
