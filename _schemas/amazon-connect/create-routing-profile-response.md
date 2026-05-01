---
description: CreateRoutingProfileResponse schema from Amazon Connect Service API
layout: schema
name: CreateRoutingProfileResponse
properties_list:
- description: The Amazon Resource Name (ARN) of the routing profile.
  name: RoutingProfileArn
  type: string
- description: The identifier of the routing profile.
  name: RoutingProfileId
  type: string
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/create-routing-profile-response-schema.json
slug: create-routing-profile-response
source_filename: create-routing-profile-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/create-routing-profile-response-schema.json\",\n  \"title\": \"CreateRoutingProfileResponse\",\n  \"description\": \"CreateRoutingProfileResponse schema from Amazon Connect Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RoutingProfileArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the routing profile.\"\n    },\n    \"RoutingProfileId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the routing profile.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-33333EXAMPLE\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/create-routing-profile-response-schema.json
tags:
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: CreateRoutingProfileResponse
---
