---
description: PutRemediationConfigurationsResponse schema
layout: schema
name: PutRemediationConfigurationsResponse
properties_list:
- description: ''
  name: FailedBatches
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-put-remediation-configurations-response-schema.json
slug: config-put-remediation-configurations-response
source_filename: config-put-remediation-configurations-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-remediation-configurations-response-schema.json\",\n  \"title\": \"PutRemediationConfigurationsResponse\",\n  \"description\": \"PutRemediationConfigurationsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FailedBatches\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailedRemediationBatches\"\n        },\n        {\n          \"description\": \"Returns a list of failed remediation batch objects.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-remediation-configurations-response-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: PutRemediationConfigurationsResponse
---
