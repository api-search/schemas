---
description: Schema representing a security or governance policy in the Apinizer platform
layout: schema
name: Apinizer Policy
properties_list:
- description: Unique identifier of the policy
  name: id
  type: string
- description: Name of the policy
  name: name
  type: string
- description: Type of policy
  name: type
  type: string
- description: Policy-specific configuration parameters
  name: configuration
  type: object
provider_name: Apinizer
provider_slug: apinizer
schema_file: json-schema/apinizer-policy-schema.json
slug: apinizer-policy
source_filename: apinizer-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apinizer/main/json-schema/apinizer-policy-schema.json\",\n  \"title\": \"Apinizer Policy\",\n  \"description\": \"Schema representing a security or governance policy in the Apinizer platform\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"Unique identifier of the policy\" },\n    \"name\": { \"type\": \"string\", \"description\": \"Name of the policy\" },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"rate-limit\", \"authentication\", \"cors\", \"ip-filter\", \"caching\", \"transformation\"],\n      \"description\": \"Type of policy\"\n    },\n    \"configuration\": { \"type\": \"object\", \"description\": \"Policy-specific configuration parameters\" }\n  },\n  \"required\": [\"id\", \"name\", \"type\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apinizer/refs/heads/main/json-schema/apinizer-policy-schema.json
tags:
- API Gateway
- API Management
- API Monitoring
- API Security
- Policies
title: Apinizer Policy
---
