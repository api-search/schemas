---
description: ComplianceIssue schema from Palo Alto Networks Prisma Cloud Compute API
layout: schema
name: ComplianceIssue
properties_list:
- description: Compliance check ID.
  name: id
  type: integer
- description: Title of the compliance check.
  name: title
  type: string
- description: Severity of the compliance issue.
  name: severity
  type: string
- description: Explanation of why the resource failed the check.
  name: cause
  type: string
- description: Detailed description of the compliance requirement.
  name: description
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-compute-api-compliance-issue-schema.json
slug: prisma-cloud-compute-api-compliance-issue
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ComplianceIssue\",\n  \"description\": \"ComplianceIssue schema from Palo Alto Networks Prisma Cloud Compute API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-compute-api-compliance-issue-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Compliance check ID.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the compliance check.\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"critical\",\n        \"high\",\n        \"medium\",\n        \"low\"\n      ],\n      \"description\": \"Severity of the compliance issue.\"\n    },\n    \"cause\": {\n      \"type\": \"string\",\n      \"description\": \"Explanation of why the resource failed the check.\"\n   \
  \ },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed description of the compliance requirement.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-compute-api-compliance-issue-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ComplianceIssue
---
