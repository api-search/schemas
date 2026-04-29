---
description: Request body for updating a policy.
layout: schema
name: PolicyUpdateRequest
properties_list:
- description: The updated display name for the policy.
  name: name
  type: string
- description: The updated status for the policy.
  name: status
  type: string
- description: Updated policy-specific configuration attributes.
  name: attributes
  type: object
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-admin-policy-update-request-schema.json
slug: atlassian-admin-policy-update-request
source_filename: atlassian-admin-policy-update-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PolicyUpdateRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for updating a policy.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The updated display name for the policy.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The updated status for the policy.\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Updated policy-specific configuration attributes.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-admin-policy-update-request-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: PolicyUpdateRequest
---
