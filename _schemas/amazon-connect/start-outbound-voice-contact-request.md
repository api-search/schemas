---
description: StartOutboundVoiceContactRequest schema from Amazon Connect Service API
layout: schema
name: StartOutboundVoiceContactRequest
properties_list:
- description: The phone number of the customer, in E.164 format.
  name: DestinationPhoneNumber
  type: string
- description: The identifier of the contact flow for the outbound call.
  name: ContactFlowId
  type: string
- description: The identifier of the Amazon Connect instance.
  name: InstanceId
  type: string
- description: Idempotency token.
  name: ClientToken
  type: string
- description: The phone number associated with the Amazon Connect instance, in E.164 format.
  name: SourcePhoneNumber
  type: string
- description: The queue for the call.
  name: QueueId
  type: string
- description: ''
  name: Attributes
  type: object
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/start-outbound-voice-contact-request-schema.json
slug: start-outbound-voice-contact-request
source_filename: start-outbound-voice-contact-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/start-outbound-voice-contact-request-schema.json\",\n  \"title\": \"StartOutboundVoiceContactRequest\",\n  \"description\": \"StartOutboundVoiceContactRequest schema from Amazon Connect Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DestinationPhoneNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The phone number of the customer, in E.164 format.\",\n      \"example\": \"+12065551212\"\n    },\n    \"ContactFlowId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the contact flow for the outbound call.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-77777EXAMPLE\"\n    },\n    \"InstanceId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the Amazon Connect instance.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-11111EXAMPLE\"\
  \n    },\n    \"ClientToken\": {\n      \"type\": \"string\",\n      \"description\": \"Idempotency token.\"\n    },\n    \"SourcePhoneNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The phone number associated with the Amazon Connect instance, in E.164 format.\"\n    },\n    \"QueueId\": {\n      \"type\": \"string\",\n      \"description\": \"The queue for the call.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-55555EXAMPLE\"\n    },\n    \"Attributes\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"ContactFlowId\",\n    \"DestinationPhoneNumber\",\n    \"InstanceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/start-outbound-voice-contact-request-schema.json
tags:
- AWS
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: StartOutboundVoiceContactRequest
---
