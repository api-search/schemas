---
description: Policy schema from Palo Alto Networks Prisma Cloud CSPM API
layout: schema
name: Policy
properties_list:
- description: Unique policy identifier.
  name: policyId
  type: string
- description: Policy name.
  name: name
  type: string
- description: Type of policy check.
  name: policyType
  type: string
- description: Policy severity level.
  name: severity
  type: string
- description: Policy description.
  name: description
  type: string
- description: Recommended remediation for policy violations.
  name: recommendation
  type: string
- description: Cloud provider the policy applies to.
  name: cloudType
  type: string
- description: Whether the policy is active.
  name: enabled
  type: boolean
- description: Whether this is a built-in policy.
  name: systemDefault
  type: boolean
- description: ''
  name: rule
  type: object
- description: ''
  name: complianceMetadata
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-cspm-api-policy-schema.json
slug: prisma-cloud-cspm-api-policy
source_filename: prisma-cloud-cspm-api-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Policy\",\n  \"description\": \"Policy schema from Palo Alto Networks Prisma Cloud CSPM API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-cspm-api-policy-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policyId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique policy identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Policy name.\"\n    },\n    \"policyType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"config\",\n        \"network\",\n        \"audit_event\",\n        \"anomaly\",\n        \"data\",\n        \"iam\"\n      ],\n      \"description\": \"Type of policy check.\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"critical\",\n        \"high\",\n        \"medium\",\n  \
  \      \"low\",\n        \"informational\"\n      ],\n      \"description\": \"Policy severity level.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Policy description.\"\n    },\n    \"recommendation\": {\n      \"type\": \"string\",\n      \"description\": \"Recommended remediation for policy violations.\"\n    },\n    \"cloudType\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud provider the policy applies to.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the policy is active.\"\n    },\n    \"systemDefault\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a built-in policy.\"\n    },\n    \"rule\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"criteria\": {\n          \"type\": \"string\",\n          \"description\": \"RQL query string.\"\n        },\n        \"type\"\
  : {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"complianceMetadata\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"standardName\": {\n            \"type\": \"string\"\n          },\n          \"requirementId\": {\n            \"type\": \"string\"\n          },\n          \"requirementName\": {\n            \"type\": \"string\"\n          },\n          \"sectionId\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-cspm-api-policy-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Policy
---
