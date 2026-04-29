---
description: Contains summary information about a routing profile.
layout: schema
name: RoutingProfileSummary
properties_list:
- description: The identifier of the routing profile.
  name: Id
  type: string
- description: The Amazon Resource Name (ARN) of the routing profile.
  name: Arn
  type: string
- description: The name of the routing profile.
  name: Name
  type: string
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/routing-profile-summary-schema.json
slug: routing-profile-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/routing-profile-summary-schema.json\",\n  \"title\": \"RoutingProfileSummary\",\n  \"description\": \"Contains summary information about a routing profile.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the routing profile.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-33333EXAMPLE\"\n    },\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the routing profile.\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the routing profile.\",\n      \"example\": \"Basic Routing Profile\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/routing-profile-summary-schema.json
tags:
- AWS
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: RoutingProfileSummary
---
