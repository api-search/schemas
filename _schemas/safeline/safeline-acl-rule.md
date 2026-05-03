---
description: An access control list rule in SafeLine WAF for blocking or allowing traffic based on conditions.
layout: schema
name: SafeLine ACL Rule
properties_list:
- description: Unique ACL rule identifier
  name: id
  type: integer
- description: Descriptive name for the rule
  name: name
  type: string
- description: Action to take when the rule matches
  name: action
  type: string
- description: List of conditions that must match to trigger the rule
  name: conditions
  type: array
- description: Whether the rule is active
  name: enabled
  type: boolean
- description: Rule creation timestamp
  name: create_time
  type: string
provider_name: SafeLine
provider_slug: safeline
schema_file: json-schema/safeline-acl-rule-schema.json
slug: safeline-acl-rule
source_filename: safeline-acl-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/safeline/main/json-schema/safeline-acl-rule-schema.json\",\n  \"title\": \"SafeLine ACL Rule\",\n  \"description\": \"An access control list rule in SafeLine WAF for blocking or allowing traffic based on conditions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique ACL rule identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Descriptive name for the rule\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"enum\": [\"block\", \"allow\", \"log\"],\n      \"description\": \"Action to take when the rule matches\"\n    },\n    \"conditions\": {\n      \"type\": \"array\",\n      \"description\": \"List of conditions that must match to trigger the rule\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\"\
  : {\n          \"field\": {\n            \"type\": \"string\",\n            \"enum\": [\"ip\", \"url\", \"method\", \"header\", \"body\", \"user_agent\", \"referer\"],\n            \"description\": \"HTTP request field to match against\"\n          },\n          \"operator\": {\n            \"type\": \"string\",\n            \"enum\": [\"equals\", \"contains\", \"startswith\", \"endswith\", \"matches\", \"in_cidr\"],\n            \"description\": \"Comparison operator\"\n          },\n          \"value\": {\n            \"type\": \"string\",\n            \"description\": \"Value to compare against\"\n          }\n        },\n        \"required\": [\"field\", \"operator\", \"value\"]\n      }\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the rule is active\"\n    },\n    \"create_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Rule creation timestamp\"\n    }\n  },\n  \"required\": [\"id\",\
  \ \"name\", \"action\", \"conditions\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/safeline/refs/heads/main/json-schema/safeline-acl-rule-schema.json
tags:
- Proxy
- WAF
- Security
- Open Source
- Reverse Proxy
- API Gateway
title: SafeLine ACL Rule
---
