---
description: Contains information about a routing profile.
layout: schema
name: RoutingProfile
properties_list:
- description: The identifier of the Amazon Connect instance.
  name: InstanceId
  type: string
- description: The name of the routing profile.
  name: Name
  type: string
- description: The Amazon Resource Name (ARN) of the routing profile.
  name: RoutingProfileArn
  type: string
- description: The identifier of the routing profile.
  name: RoutingProfileId
  type: string
- description: The description of the routing profile.
  name: Description
  type: string
- description: ''
  name: MediaConcurrencies
  type: array
- description: The identifier of the default outbound queue for this routing profile.
  name: DefaultOutboundQueueId
  type: string
- description: ''
  name: Tags
  type: object
- description: The number of associated queues in routing profile.
  name: NumberOfAssociatedQueues
  type: integer
- description: The number of associated users in routing profile.
  name: NumberOfAssociatedUsers
  type: integer
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/routing-profile-schema.json
slug: routing-profile
source_filename: routing-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/routing-profile-schema.json\",\n  \"title\": \"RoutingProfile\",\n  \"description\": \"Contains information about a routing profile.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the Amazon Connect instance.\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the routing profile.\",\n      \"example\": \"Voice Agents\"\n    },\n    \"RoutingProfileArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the routing profile.\"\n    },\n    \"RoutingProfileId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the routing profile.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-33333EXAMPLE\"\n    },\n\
  \    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the routing profile.\"\n    },\n    \"MediaConcurrencies\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MediaConcurrency\"\n      }\n    },\n    \"DefaultOutboundQueueId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the default outbound queue for this routing profile.\"\n    },\n    \"Tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"NumberOfAssociatedQueues\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of associated queues in routing profile.\"\n    },\n    \"NumberOfAssociatedUsers\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of associated users in routing profile.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/routing-profile-schema.json
tags:
- AWS
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: RoutingProfile
---
