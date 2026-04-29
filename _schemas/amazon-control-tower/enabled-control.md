---
description: Information about an enabled control.
layout: schema
name: EnabledControl
properties_list:
- description: The ARN of the enabled control.
  name: arn
  type: string
- description: The control identifier.
  name: controlIdentifier
  type: string
- description: ''
  name: driftStatusSummary
  type: object
- description: ''
  name: parameters
  type: array
- description: ''
  name: statusSummary
  type: object
- description: The ARN of the organizational unit.
  name: targetIdentifier
  type: string
provider_name: Amazon Control Tower
provider_slug: amazon-control-tower
schema_file: json-schema/enabled-control-schema.json
slug: enabled-control
source_filename: enabled-control-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/enabled-control-schema.json\",\n  \"title\": \"EnabledControl\",\n  \"description\": \"Information about an enabled control.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the enabled control.\",\n      \"example\": \"arn:aws:controltower:us-east-1:123456789012:enabledcontrol/a1b2c3d4EXAMPLE\"\n    },\n    \"controlIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The control identifier.\",\n      \"example\": \"arn:aws:controltower:us-east-1::control/AWS-GR_ENCRYPTED_VOLUMES\"\n    },\n    \"driftStatusSummary\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"driftStatus\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"DRIFTED\",\n            \"IN_SYNC\"\
  ,\n            \"NOT_CHECKING_FOR_DRIFT\",\n            \"UNKNOWN\"\n          ]\n        }\n      }\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/EnabledControlParameter\"\n      }\n    },\n    \"statusSummary\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"lastOperationIdentifier\": {\n          \"type\": \"string\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"SUCCEEDED\",\n            \"FAILED\",\n            \"UNDER_CHANGE\"\n          ]\n        }\n      }\n    },\n    \"targetIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the organizational unit.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/enabled-control-schema.json
tags:
- AWS
- Compliance
- Governance
- Landing Zone
- Multi-Account
- Security
- Controls
title: EnabledControl
---
