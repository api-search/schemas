---
description: Policy schema from Amazon Organizations
layout: schema
name: Policy
properties_list:
- description: ''
  name: PolicySummary
  type: object
- description: ''
  name: Content
  type: string
provider_name: Amazon Organizations
provider_slug: amazon-organizations
schema_file: json-schema/openapi-policy-schema.json
slug: openapi-policy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-organizations/refs/heads/main/json-schema/openapi-policy-schema.json\",\n  \"title\": \"Policy\",\n  \"description\": \"Policy schema from Amazon Organizations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PolicySummary\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Id\": {\n          \"type\": \"string\"\n        },\n        \"Arn\": {\n          \"type\": \"string\"\n        },\n        \"Name\": {\n          \"type\": \"string\"\n        },\n        \"Type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"SERVICE_CONTROL_POLICY\",\n            \"TAG_POLICY\",\n            \"BACKUP_POLICY\",\n            \"AISERVICES_OPT_OUT_POLICY\"\n          ]\n        }\n      }\n    },\n    \"Content\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-organizations/refs/heads/main/json-schema/openapi-policy-schema.json
tags:
- Account Management
- AWS
- Consolidated Billing
- Governance
- Multi-Account
- Organizations
- Policies
title: Policy
---
