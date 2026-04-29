---
description: CreateRoutingProfileRequest schema from Amazon Connect Service API
layout: schema
name: CreateRoutingProfileRequest
properties_list:
- description: The name of the routing profile. Must not be more than 127 characters.
  name: Name
  type: string
- description: Description of the routing profile.
  name: Description
  type: string
- description: The default outbound queue for the routing profile.
  name: DefaultOutboundQueueId
  type: string
- description: ''
  name: QueueConfigs
  type: array
- description: ''
  name: MediaConcurrencies
  type: array
- description: ''
  name: Tags
  type: object
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/create-routing-profile-request-schema.json
slug: create-routing-profile-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/create-routing-profile-request-schema.json\",\n  \"title\": \"CreateRoutingProfileRequest\",\n  \"description\": \"CreateRoutingProfileRequest schema from Amazon Connect Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the routing profile. Must not be more than 127 characters.\",\n      \"example\": \"Voice Agents\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the routing profile.\",\n      \"example\": \"Routing profile for voice agents\"\n    },\n    \"DefaultOutboundQueueId\": {\n      \"type\": \"string\",\n      \"description\": \"The default outbound queue for the routing profile.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-55555EXAMPLE\"\n \
  \   },\n    \"QueueConfigs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"QueueReference\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"QueueId\": {\n                \"type\": \"string\"\n              },\n              \"Channel\": {\n                \"type\": \"string\"\n              }\n            }\n          },\n          \"Priority\": {\n            \"type\": \"integer\"\n          },\n          \"Delay\": {\n            \"type\": \"integer\"\n          }\n        }\n      }\n    },\n    \"MediaConcurrencies\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MediaConcurrency\"\n      }\n    },\n    \"Tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"DefaultOutboundQueueId\",\n    \"Description\",\n    \"MediaConcurrencies\"\
  ,\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/create-routing-profile-request-schema.json
tags:
- AWS
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: CreateRoutingProfileRequest
---
