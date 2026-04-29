---
description: AccessPolicyRequest schema from Palo Alto Networks SASE IAM Service API
layout: schema
name: AccessPolicyRequest
properties_list:
- description: ID of the service account or user to grant access to.
  name: principal_id
  type: string
- description: Type of principal.
  name: principal_type
  type: string
- description: ID of the role to assign.
  name: role_id
  type: string
- description: TSG scope for this policy.
  name: tsg_id
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-iam-api-access-policy-request-schema.json
slug: sase-iam-api-access-policy-request
source_filename: sase-iam-api-access-policy-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccessPolicyRequest\",\n  \"description\": \"AccessPolicyRequest schema from Palo Alto Networks SASE IAM Service API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-iam-api-access-policy-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"principal_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the service account or user to grant access to.\"\n    },\n    \"principal_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"service_account\",\n        \"user\"\n      ],\n      \"description\": \"Type of principal.\"\n    },\n    \"role_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the role to assign.\"\n    },\n    \"tsg_id\": {\n      \"type\": \"string\",\n      \"description\": \"TSG scope for this policy.\"\n    }\n  },\n  \"required\": [\n\
  \    \"principal_id\",\n    \"principal_type\",\n    \"role_id\",\n    \"tsg_id\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-iam-api-access-policy-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: AccessPolicyRequest
---
