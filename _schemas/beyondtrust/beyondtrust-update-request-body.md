---
description: Request body for approving, denying, or cancelling a request.
layout: schema
name: UpdateRequestBody
properties_list:
- description: The action to perform on the request.
  name: Action
  type: string
- description: Reason for the action.
  name: Reason
  type: string
provider_name: BeyondTrust
provider_slug: beyondtrust
schema_file: json-schema/beyondtrust-update-request-body-schema.json
slug: beyondtrust-update-request-body
source_filename: beyondtrust-update-request-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/beyondtrust/refs/heads/main/json-schema/beyondtrust-update-request-body-schema.json\",\n  \"title\": \"UpdateRequestBody\",\n  \"description\": \"Request body for approving, denying, or cancelling a request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Action\": {\n      \"type\": \"string\",\n      \"description\": \"The action to perform on the request.\",\n      \"enum\": [\n        \"Approve\",\n        \"Deny\",\n        \"Cancel\"\n      ],\n      \"example\": \"Approve\"\n    },\n    \"Reason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for the action.\",\n      \"example\": \"Approved for maintenance window\"\n    }\n  },\n  \"required\": [\n    \"Action\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/beyondtrust/refs/heads/main/json-schema/beyondtrust-update-request-body-schema.json
tags:
- Access
- Access Management
- Compliance
- Credentials
- Privileged Access
- Security
- Secrets
- Zero Trust
title: UpdateRequestBody
---
