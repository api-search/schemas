---
description: EnableControlRequest schema from AWS Control Tower API
layout: schema
name: EnableControlRequest
properties_list:
- description: The ARN of the control. Only Strongly recommended and Elective controls are permitted.
  name: controlIdentifier
  type: string
- description: The ARN of the organizational unit on which the control will be enabled.
  name: targetIdentifier
  type: string
- description: A list of input parameter values that are supplied to enable the control.
  name: parameters
  type: array
- description: Tags to apply to the EnabledControl resource.
  name: tags
  type: object
provider_name: Amazon Control Tower
provider_slug: amazon-control-tower
schema_file: json-schema/enable-control-request-schema.json
slug: enable-control-request
source_filename: enable-control-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/enable-control-request-schema.json\",\n  \"title\": \"EnableControlRequest\",\n  \"description\": \"EnableControlRequest schema from AWS Control Tower API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"controlIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the control. Only Strongly recommended and Elective controls are permitted.\",\n      \"example\": \"arn:aws:controltower:us-east-1::control/AWS-GR_ENCRYPTED_VOLUMES\"\n    },\n    \"targetIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the organizational unit on which the control will be enabled.\",\n      \"example\": \"arn:aws:organizations::123456789012:ou/o-exampleorgid11/ou-exampleouid111\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"A list of input parameter values that are supplied to enable the control.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/EnabledControlParameter\"\n      }\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Tags to apply to the EnabledControl resource.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"controlIdentifier\",\n    \"targetIdentifier\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/enable-control-request-schema.json
tags:
- Compliance
- Governance
- Landing Zone
- Multi-Account
- Security
- Controls
title: EnableControlRequest
---
