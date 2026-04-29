---
description: AccessPolicy schema from Palo Alto Networks SASE IAM Service API
layout: schema
name: AccessPolicy
properties_list:
- description: Unique identifier of the access policy.
  name: id
  type: string
- description: ID of the service account or user this policy applies to.
  name: principal_id
  type: string
- description: Type of principal.
  name: principal_type
  type: string
- description: ID of the role assigned by this policy.
  name: role_id
  type: string
- description: Name of the role assigned.
  name: role_name
  type: string
- description: TSG scope this policy applies to.
  name: tsg_id
  type: string
- description: ''
  name: created_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-iam-api-access-policy-schema.json
slug: sase-iam-api-access-policy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccessPolicy\",\n  \"description\": \"AccessPolicy schema from Palo Alto Networks SASE IAM Service API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-iam-api-access-policy-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the access policy.\"\n    },\n    \"principal_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the service account or user this policy applies to.\"\n    },\n    \"principal_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"service_account\",\n        \"user\"\n      ],\n      \"description\": \"Type of principal.\"\n    },\n    \"role_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the role assigned by this policy.\"\n    },\n    \"role_name\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Name of the role assigned.\"\n    },\n    \"tsg_id\": {\n      \"type\": \"string\",\n      \"description\": \"TSG scope this policy applies to.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-iam-api-access-policy-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: AccessPolicy
---
