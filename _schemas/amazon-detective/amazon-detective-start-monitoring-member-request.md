---
description: Request to start monitoring a member account
layout: schema
name: StartMonitoringMemberRequest
properties_list:
- description: The ARN of the behavior graph.
  name: GraphArn
  type: string
- description: The account ID of the member account to try to enable.
  name: AccountId
  type: string
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-start-monitoring-member-request-schema.json
slug: amazon-detective-start-monitoring-member-request
source_filename: amazon-detective-start-monitoring-member-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-start-monitoring-member-request-schema.json\",\n  \"title\": \"StartMonitoringMemberRequest\",\n  \"description\": \"Request to start monitoring a member account\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GraphArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the behavior graph.\",\n      \"example\": \"arn:aws:detective:us-east-1:123456789012:graph:abc123def456\"\n    },\n    \"AccountId\": {\n      \"type\": \"string\",\n      \"description\": \"The account ID of the member account to try to enable.\",\n      \"example\": \"234567890123\"\n    }\n  },\n  \"required\": [\n    \"GraphArn\",\n    \"AccountId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-start-monitoring-member-request-schema.json
tags:
- Forensics
- Investigation
- Security
title: StartMonitoringMemberRequest
---
