---
description: The Amazon Connect instance.
layout: schema
name: Instance
properties_list:
- description: The identifier of the Amazon Connect instance.
  name: Id
  type: string
- description: The Amazon Resource Name (ARN) of the instance.
  name: Arn
  type: string
- description: The identity management type.
  name: IdentityManagementType
  type: string
- description: The alias of the instance.
  name: InstanceAlias
  type: string
- description: When the instance was created.
  name: CreatedTime
  type: string
- description: The service role of the instance.
  name: ServiceRole
  type: string
- description: The state of the instance.
  name: InstanceStatus
  type: string
- description: Whether inbound calls are enabled.
  name: InboundCallsEnabled
  type: boolean
- description: Whether outbound calls are enabled.
  name: OutboundCallsEnabled
  type: boolean
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/instance-schema.json
slug: instance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/instance-schema.json\",\n  \"title\": \"Instance\",\n  \"description\": \"The Amazon Connect instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the Amazon Connect instance.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-11111EXAMPLE\"\n    },\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the instance.\",\n      \"example\": \"arn:aws:connect:us-east-1:123456789012:instance/a1b2c3d4-5678-90ab-cdef-11111EXAMPLE\"\n    },\n    \"IdentityManagementType\": {\n      \"type\": \"string\",\n      \"description\": \"The identity management type.\",\n      \"enum\": [\n        \"SAML\",\n        \"CONNECT_MANAGED\",\n        \"EXISTING_DIRECTORY\"\n      ],\n\
  \      \"example\": \"CONNECT_MANAGED\"\n    },\n    \"InstanceAlias\": {\n      \"type\": \"string\",\n      \"description\": \"The alias of the instance.\",\n      \"example\": \"my-contact-center\"\n    },\n    \"CreatedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the instance was created.\",\n      \"example\": \"2025-01-15T10:30:00Z\"\n    },\n    \"ServiceRole\": {\n      \"type\": \"string\",\n      \"description\": \"The service role of the instance.\"\n    },\n    \"InstanceStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The state of the instance.\",\n      \"enum\": [\n        \"CREATION_IN_PROGRESS\",\n        \"ACTIVE\",\n        \"CREATION_FAILED\"\n      ],\n      \"example\": \"ACTIVE\"\n    },\n    \"InboundCallsEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether inbound calls are enabled.\",\n      \"example\": true\n    },\n    \"OutboundCallsEnabled\": {\n      \"type\"\
  : \"boolean\",\n      \"description\": \"Whether outbound calls are enabled.\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/instance-schema.json
tags:
- AWS
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: Instance
---
