---
description: ListRoutingProfilesResponse schema from Amazon Connect Service API
layout: schema
name: ListRoutingProfilesResponse
properties_list:
- description: ''
  name: RoutingProfileSummaryList
  type: array
- description: ''
  name: NextToken
  type: string
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/list-routing-profiles-response-schema.json
slug: list-routing-profiles-response
source_filename: list-routing-profiles-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/list-routing-profiles-response-schema.json\",\n  \"title\": \"ListRoutingProfilesResponse\",\n  \"description\": \"ListRoutingProfilesResponse schema from Amazon Connect Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RoutingProfileSummaryList\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/RoutingProfileSummary\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/list-routing-profiles-response-schema.json
tags:
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: ListRoutingProfilesResponse
---
