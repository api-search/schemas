---
description: Organization schema from Amazon Organizations
layout: schema
name: Organization
properties_list:
- description: ''
  name: Id
  type: string
- description: ''
  name: Arn
  type: string
- description: ''
  name: FeatureSet
  type: string
- description: ''
  name: MasterAccountArn
  type: string
- description: ''
  name: MasterAccountId
  type: string
- description: ''
  name: MasterAccountEmail
  type: string
provider_name: Amazon Organizations
provider_slug: amazon-organizations
schema_file: json-schema/openapi-organization-schema.json
slug: openapi-organization
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-organizations/refs/heads/main/json-schema/openapi-organization-schema.json\",\n  \"title\": \"Organization\",\n  \"description\": \"Organization schema from Amazon Organizations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\"\n    },\n    \"Arn\": {\n      \"type\": \"string\"\n    },\n    \"FeatureSet\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ALL\",\n        \"CONSOLIDATED_BILLING\"\n      ]\n    },\n    \"MasterAccountArn\": {\n      \"type\": \"string\"\n    },\n    \"MasterAccountId\": {\n      \"type\": \"string\"\n    },\n    \"MasterAccountEmail\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-organizations/refs/heads/main/json-schema/openapi-organization-schema.json
tags:
- Account Management
- AWS
- Consolidated Billing
- Governance
- Multi-Account
- Organizations
- Policies
title: Organization
---
