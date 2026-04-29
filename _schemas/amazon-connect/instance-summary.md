---
description: Information about the Amazon Connect instance.
layout: schema
name: InstanceSummary
properties_list:
- description: The identifier of the instance.
  name: Id
  type: string
- description: The ARN of the instance.
  name: Arn
  type: string
- description: The identity management type.
  name: IdentityManagementType
  type: string
- description: The alias of the instance.
  name: InstanceAlias
  type: string
- description: The state of the instance.
  name: InstanceStatus
  type: string
- description: ''
  name: InboundCallsEnabled
  type: boolean
- description: ''
  name: OutboundCallsEnabled
  type: boolean
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/instance-summary-schema.json
slug: instance-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/instance-summary-schema.json\",\n  \"title\": \"InstanceSummary\",\n  \"description\": \"Information about the Amazon Connect instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the instance.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-11111EXAMPLE\"\n    },\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the instance.\",\n      \"example\": \"arn:aws:connect:us-east-1:123456789012:instance/a1b2c3d4-5678-90ab-cdef-11111EXAMPLE\"\n    },\n    \"IdentityManagementType\": {\n      \"type\": \"string\",\n      \"description\": \"The identity management type.\",\n      \"example\": \"CONNECT_MANAGED\"\n    },\n    \"InstanceAlias\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The alias of the instance.\",\n      \"example\": \"my-contact-center\"\n    },\n    \"InstanceStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The state of the instance.\",\n      \"example\": \"ACTIVE\"\n    },\n    \"InboundCallsEnabled\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"OutboundCallsEnabled\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/instance-summary-schema.json
tags:
- AWS
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: InstanceSummary
---
