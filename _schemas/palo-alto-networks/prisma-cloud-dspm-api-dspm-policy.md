---
description: DSPMPolicy schema from Palo Alto Networks Prisma Cloud DSPM API
layout: schema
name: DSPMPolicy
properties_list:
- description: Unique DSPM policy identifier.
  name: id
  type: string
- description: Policy name.
  name: name
  type: string
- description: Policy description.
  name: description
  type: string
- description: Whether the policy is currently active.
  name: enabled
  type: boolean
- description: Severity level of violations detected by this policy.
  name: severity
  type: string
- description: Classification label this policy governs.
  name: classification
  type: string
- description: Security controls required for data matching this policy.
  name: requiredControls
  type: array
- description: Cloud providers this policy applies to.
  name: cloudProviders
  type: array
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-dspm-api-dspm-policy-schema.json
slug: prisma-cloud-dspm-api-dspm-policy
source_filename: prisma-cloud-dspm-api-dspm-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DSPMPolicy\",\n  \"description\": \"DSPMPolicy schema from Palo Alto Networks Prisma Cloud DSPM API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-dspm-api-dspm-policy-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique DSPM policy identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Policy name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Policy description.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the policy is currently active.\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"critical\",\n        \"high\",\n        \"medium\",\n        \"low\"\n    \
  \  ],\n      \"description\": \"Severity level of violations detected by this policy.\"\n    },\n    \"classification\": {\n      \"type\": \"string\",\n      \"description\": \"Classification label this policy governs.\"\n    },\n    \"requiredControls\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"encryption\",\n          \"accessRestriction\",\n          \"auditLogging\",\n          \"backup\",\n          \"networkIsolation\"\n        ]\n      },\n      \"description\": \"Security controls required for data matching this policy.\"\n    },\n    \"cloudProviders\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"aws\",\n          \"azure\",\n          \"gcp\"\n        ]\n      },\n      \"description\": \"Cloud providers this policy applies to.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\"\
  : true\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-dspm-api-dspm-policy-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: DSPMPolicy
---
