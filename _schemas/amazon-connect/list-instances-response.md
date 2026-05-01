---
description: ListInstancesResponse schema from Amazon Connect Service API
layout: schema
name: ListInstancesResponse
properties_list:
- description: ''
  name: InstanceSummaryList
  type: array
- description: If there are additional results, this is the token for the next set.
  name: NextToken
  type: string
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/list-instances-response-schema.json
slug: list-instances-response
source_filename: list-instances-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/list-instances-response-schema.json\",\n  \"title\": \"ListInstancesResponse\",\n  \"description\": \"ListInstancesResponse schema from Amazon Connect Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceSummaryList\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/InstanceSummary\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"If there are additional results, this is the token for the next set.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/list-instances-response-schema.json
tags:
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: ListInstancesResponse
---
