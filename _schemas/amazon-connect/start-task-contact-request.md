---
description: StartTaskContactRequest schema from Amazon Connect Service API
layout: schema
name: StartTaskContactRequest
properties_list:
- description: The identifier of the Amazon Connect instance.
  name: InstanceId
  type: string
- description: The identifier of the previous chat, voice, or task contact.
  name: PreviousContactId
  type: string
- description: The identifier of the contact flow for initiating the tasks.
  name: ContactFlowId
  type: string
- description: ''
  name: Attributes
  type: object
- description: The name of a task that is shown to an agent in the Contact Control Panel (CCP).
  name: Name
  type: string
- description: ''
  name: References
  type: object
- description: A description of the task that is shown to an agent in the Contact Control Panel.
  name: Description
  type: string
- description: ''
  name: ClientToken
  type: string
- description: ''
  name: ScheduledTime
  type: string
- description: ''
  name: TaskTemplateId
  type: string
- description: ''
  name: QuickConnectId
  type: string
- description: ''
  name: RelatedContactId
  type: string
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/start-task-contact-request-schema.json
slug: start-task-contact-request
source_filename: start-task-contact-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/start-task-contact-request-schema.json\",\n  \"title\": \"StartTaskContactRequest\",\n  \"description\": \"StartTaskContactRequest schema from Amazon Connect Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the Amazon Connect instance.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-11111EXAMPLE\"\n    },\n    \"PreviousContactId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the previous chat, voice, or task contact.\"\n    },\n    \"ContactFlowId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the contact flow for initiating the tasks.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-77777EXAMPLE\"\n    },\n    \"Attributes\": {\n   \
  \   \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of a task that is shown to an agent in the Contact Control Panel (CCP).\",\n      \"example\": \"Follow-up with customer\"\n    },\n    \"References\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"object\"\n      }\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the task that is shown to an agent in the Contact Control Panel.\",\n      \"example\": \"Call customer back regarding their support case\"\n    },\n    \"ClientToken\": {\n      \"type\": \"string\"\n    },\n    \"ScheduledTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"TaskTemplateId\": {\n      \"type\": \"string\"\n    },\n    \"QuickConnectId\": {\n      \"type\": \"string\"\n    },\n    \"RelatedContactId\"\
  : {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"InstanceId\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/start-task-contact-request-schema.json
tags:
- AWS
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: StartTaskContactRequest
---
