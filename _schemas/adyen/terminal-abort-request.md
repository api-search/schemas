---
description: It conveys Information requested for identification of the message request carrying the transaction to abort. A message to display on the CustomerError Device could be sent by the Sale System (DisplayOutput). Body of the Abort Request message.
layout: schema
name: AbortRequest
properties_list:
- description: ''
  name: MessageReference
  type: object
- description: Reason of aborting a transaction.
  name: AbortReason
  type: string
- description: ''
  name: DisplayOutput
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-abort-request-schema.json
slug: terminal-abort-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-abort-request-schema.json\",\n  \"title\": \"AbortRequest\",\n  \"description\": \"It conveys Information requested for identification of the message request carrying the transaction to abort. A message to display on the CustomerError Device could be sent by the Sale System (DisplayOutput). Body of the Abort Request message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MessageReference\": {\n      \"$ref\": \"#/components/schemas/MessageReference\"\n    },\n    \"AbortReason\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"Reason of aborting a transaction.\"\n    },\n    \"DisplayOutput\": {\n      \"$ref\": \"#/components/schemas/DisplayOutput\"\n    }\n  },\n  \"required\": [\n    \"MessageReference\",\n    \"AbortReason\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-abort-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AbortRequest
---
