---
description: OperationStatus schema from Adyen API
layout: schema
name: OperationStatus
properties_list:
- description: The message regarding the operation status.
  name: message
  type: object
- description: The status code.
  name: statusCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-operation-status-schema.json
slug: notifications-operation-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-operation-status-schema.json\",\n  \"title\": \"OperationStatus\",\n  \"description\": \"OperationStatus schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"description\": \"The message regarding the operation status.\",\n      \"$ref\": \"#/components/schemas/Message\"\n    },\n    \"statusCode\": {\n      \"description\": \"The status code.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-operation-status-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: OperationStatus
---
