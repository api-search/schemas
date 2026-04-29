---
description: Represents an organization-level policy that defines rules and controls for security, authentication, and governance.
layout: schema
name: Policy
properties_list:
- description: The unique identifier of the policy.
  name: id
  type: string
- description: The type of policy.
  name: type
  type: string
- description: The display name of the policy.
  name: name
  type: string
- description: The current status of the policy.
  name: status
  type: string
- description: Policy-specific configuration attributes.
  name: attributes
  type: object
- description: Resources this policy applies to.
  name: resources
  type: array
- description: When the policy was created.
  name: created
  type: string
- description: When the policy was last updated.
  name: updated
  type: string
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-admin-policy-schema.json
slug: atlassian-admin-policy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Policy\",\n  \"type\": \"object\",\n  \"description\": \"Represents an organization-level policy that defines rules and controls for security, authentication, and governance.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the policy.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of policy.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the policy.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the policy.\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Policy-specific configuration attributes.\"\n    },\n    \"resources\": {\n      \"type\": \"array\",\n      \"description\": \"Resources this policy applies to.\"\n    },\n  \
  \  \"created\": {\n      \"type\": \"string\",\n      \"description\": \"When the policy was created.\"\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"description\": \"When the policy was last updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-admin-policy-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: Policy
---
