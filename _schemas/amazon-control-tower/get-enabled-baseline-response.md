---
description: GetEnabledBaselineResponse schema from AWS Control Tower API
layout: schema
name: GetEnabledBaselineResponse
properties_list:
- description: ''
  name: enabledBaselineDetails
  type: object
provider_name: Amazon Control Tower
provider_slug: amazon-control-tower
schema_file: json-schema/get-enabled-baseline-response-schema.json
slug: get-enabled-baseline-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/get-enabled-baseline-response-schema.json\",\n  \"title\": \"GetEnabledBaselineResponse\",\n  \"description\": \"GetEnabledBaselineResponse schema from AWS Control Tower API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabledBaselineDetails\": {\n      \"$ref\": \"#/components/schemas/EnabledBaseline\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/get-enabled-baseline-response-schema.json
tags:
- AWS
- Compliance
- Governance
- Landing Zone
- Multi-Account
- Security
- Controls
title: GetEnabledBaselineResponse
---
