---
description: CreateInstanceRequest schema from Amazon Connect Service API
layout: schema
name: CreateInstanceRequest
properties_list:
- description: The idempotency token.
  name: ClientToken
  type: string
- description: The type of identity management for your Amazon Connect users.
  name: IdentityManagementType
  type: string
- description: The name for your instance.
  name: InstanceAlias
  type: string
- description: The identifier for the directory.
  name: DirectoryId
  type: string
- description: Your contact center handles incoming contacts.
  name: InboundCallsEnabled
  type: boolean
- description: Your contact center allows outbound calls.
  name: OutboundCallsEnabled
  type: boolean
- description: The tags used to organize, track, or control access for this resource.
  name: Tags
  type: object
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/create-instance-request-schema.json
slug: create-instance-request
source_filename: create-instance-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/create-instance-request-schema.json\",\n  \"title\": \"CreateInstanceRequest\",\n  \"description\": \"CreateInstanceRequest schema from Amazon Connect Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClientToken\": {\n      \"type\": \"string\",\n      \"description\": \"The idempotency token.\"\n    },\n    \"IdentityManagementType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of identity management for your Amazon Connect users.\",\n      \"enum\": [\n        \"SAML\",\n        \"CONNECT_MANAGED\",\n        \"EXISTING_DIRECTORY\"\n      ],\n      \"example\": \"CONNECT_MANAGED\"\n    },\n    \"InstanceAlias\": {\n      \"type\": \"string\",\n      \"description\": \"The name for your instance.\",\n      \"example\": \"my-contact-center\"\n    },\n    \"DirectoryId\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The identifier for the directory.\"\n    },\n    \"InboundCallsEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Your contact center handles incoming contacts.\",\n      \"example\": true\n    },\n    \"OutboundCallsEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Your contact center allows outbound calls.\",\n      \"example\": true\n    },\n    \"Tags\": {\n      \"type\": \"object\",\n      \"description\": \"The tags used to organize, track, or control access for this resource.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"IdentityManagementType\",\n    \"InboundCallsEnabled\",\n    \"OutboundCallsEnabled\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/create-instance-request-schema.json
tags:
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: CreateInstanceRequest
---
