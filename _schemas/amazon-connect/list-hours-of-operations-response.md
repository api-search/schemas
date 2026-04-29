---
description: ListHoursOfOperationsResponse schema from Amazon Connect Service API
layout: schema
name: ListHoursOfOperationsResponse
properties_list:
- description: ''
  name: HoursOfOperationSummaryList
  type: array
- description: ''
  name: NextToken
  type: string
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/list-hours-of-operations-response-schema.json
slug: list-hours-of-operations-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/list-hours-of-operations-response-schema.json\",\n  \"title\": \"ListHoursOfOperationsResponse\",\n  \"description\": \"ListHoursOfOperationsResponse schema from Amazon Connect Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HoursOfOperationSummaryList\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/HoursOfOperationSummary\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/list-hours-of-operations-response-schema.json
tags:
- AWS
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: ListHoursOfOperationsResponse
---
